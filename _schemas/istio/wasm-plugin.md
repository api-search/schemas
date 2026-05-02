---
description: A WasmPlugin provides a mechanism to extend the functionality provided by the Istio proxy through WebAssembly filters. It enables custom authentication, authorization, metrics, logging, and traffic transformation at the proxy level.
layout: schema
name: Istio WasmPlugin
properties_list:
- description: Workload selector to apply the plugin to specific workloads.
  name: selector
  type: object
- description: Target references to apply the plugin to specific resources.
  name: targetRefs
  type: array
- description: URL of a Wasm module or OCI container image. Supports oci://, http://, https://, and file:// schemes.
  name: url
  type: string
- description: SHA256 checksum that will be used to verify the Wasm module or OCI container.
  name: sha256
  type: string
- description: The pull behavior to be applied when fetching Wasm module images.
  name: imagePullPolicy
  type: string
- description: Credentials to use for OCI image pulling. Name of a Kubernetes Secret.
  name: imagePullSecret
  type: string
- description: The configuration that will be passed on to the plugin. Encoded as JSON and passed to the Wasm module.
  name: pluginConfig
  type: object
- description: The plugin name to be used in the Envoy configuration. Allows distinguishing between multiple uses of the same Wasm module.
  name: pluginName
  type: string
- description: Determines where in the filter chain this WasmPlugin is to be injected.
  name: phase
  type: string
- description: Determines ordering of WasmPlugins in the same phase. Higher priority is evaluated first.
  name: priority
  type: integer
- description: Specifies the failure behavior for the plugin. FAIL_CLOSE rejects traffic, FAIL_OPEN skips the plugin.
  name: failStrategy
  type: string
- description: Configuration for the Wasm VM.
  name: vmConfig
  type: object
- description: Specifies the criteria to determine which traffic is passed to WasmPlugin.
  name: match
  type: array
- description: Specifies the type of Wasm Extension to be used.
  name: type
  type: string
provider_name: Istio
provider_slug: istio
schema_file: json-schema/wasm-plugin.json
slug: wasm-plugin
source_filename: wasm-plugin.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/istio/blob/main/json-schema/wasm-plugin.json\",\n  \"title\": \"Istio WasmPlugin\",\n  \"description\": \"A WasmPlugin provides a mechanism to extend the functionality provided by the Istio proxy through WebAssembly filters. It enables custom authentication, authorization, metrics, logging, and traffic transformation at the proxy level.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"selector\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"matchLabels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"One or more labels that indicate a specific set of pods/VMs on which the plugin should be applied.\"\n        }\n      },\n      \"description\": \"Workload selector to apply the plugin to specific workloads.\"\n    },\n    \"targetRefs\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"group\": {\n            \"type\": \"string\"\n          },\n          \"kind\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"Target references to apply the plugin to specific resources.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of a Wasm module or OCI container image. Supports oci://, http://, https://, and file:// schemes.\"\n    },\n    \"sha256\": {\n      \"type\": \"string\",\n      \"description\": \"SHA256 checksum that will be used to verify the Wasm module or OCI container.\"\n    },\n    \"imagePullPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\"UNSPECIFIED_POLICY\", \"IfNotPresent\", \"Always\"],\n      \"description\": \"The pull behavior to be applied when fetching Wasm module\
  \ images.\"\n    },\n    \"imagePullSecret\": {\n      \"type\": \"string\",\n      \"description\": \"Credentials to use for OCI image pulling. Name of a Kubernetes Secret.\"\n    },\n    \"pluginConfig\": {\n      \"type\": \"object\",\n      \"description\": \"The configuration that will be passed on to the plugin. Encoded as JSON and passed to the Wasm module.\"\n    },\n    \"pluginName\": {\n      \"type\": \"string\",\n      \"description\": \"The plugin name to be used in the Envoy configuration. Allows distinguishing between multiple uses of the same Wasm module.\"\n    },\n    \"phase\": {\n      \"type\": \"string\",\n      \"enum\": [\"UNSPECIFIED_PHASE\", \"AUTHN\", \"AUTHZ\", \"STATS\"],\n      \"description\": \"Determines where in the filter chain this WasmPlugin is to be injected.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Determines ordering of WasmPlugins in the same phase. Higher priority is evaluated first.\"\n    },\n  \
  \  \"failStrategy\": {\n      \"type\": \"string\",\n      \"enum\": [\"FAIL_CLOSE\", \"FAIL_OPEN\"],\n      \"description\": \"Specifies the failure behavior for the plugin. FAIL_CLOSE rejects traffic, FAIL_OPEN skips the plugin.\"\n    },\n    \"vmConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for the Wasm VM.\",\n      \"properties\": {\n        \"env\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Name of the environment variable.\"\n              },\n              \"valueFrom\": {\n                \"type\": \"string\",\n                \"enum\": [\"INLINE\", \"HOST\"],\n                \"description\": \"Source for the environment variable's value.\"\n              },\n              \"value\": {\n                \"type\": \"string\",\n                \"description\": \"\
  Value for the environment variable when valueFrom is INLINE.\"\n              }\n            },\n            \"required\": [\"name\"]\n          },\n          \"description\": \"Environment variables to pass to the VM.\"\n        }\n      }\n    },\n    \"match\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"mode\": {\n            \"type\": \"string\",\n            \"enum\": [\"UNDEFINED\", \"CLIENT\", \"SERVER\", \"CLIENT_AND_SERVER\"],\n            \"description\": \"Criteria for selecting traffic by their direction.\"\n          },\n          \"ports\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"number\": {\n                  \"type\": \"integer\"\n                }\n              }\n            },\n            \"description\": \"Criteria for selecting traffic by port.\"\n          }\n        }\n     \
  \ },\n      \"description\": \"Specifies the criteria to determine which traffic is passed to WasmPlugin.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"UNSPECIFIED_PLUGIN_TYPE\", \"HTTP\", \"NETWORK\"],\n      \"description\": \"Specifies the type of Wasm Extension to be used.\"\n    }\n  },\n  \"required\": [\"url\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/json-schema/wasm-plugin.json
tags:
- CNCF
- Kubernetes
- Microservices
- Open Source
- Service Mesh
title: Istio WasmPlugin
---
