---
description: GatewayParameters customizes gateway infrastructure deployment settings including replicas, container configuration, and proxy provisioning.
layout: schema
name: kgateway GatewayParameters
properties_list:
- description: API version for the GatewayParameters resource.
  name: apiVersion
  type: string
- description: Resource kind.
  name: kind
  type: string
- description: Standard Kubernetes object metadata.
  name: metadata
  type: object
- description: GatewayParametersSpec defines the desired state of GatewayParameters.
  name: spec
  type: object
provider_name: Kgateway
provider_slug: kgateway
schema_file: json-schema/gateway-parameters.json
slug: gateway-parameters
source_filename: gateway-parameters.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kgateway/blob/main/json-schema/gateway-parameters.json\",\n  \"title\": \"kgateway GatewayParameters\",\n  \"description\": \"GatewayParameters customizes gateway infrastructure deployment settings including replicas, container configuration, and proxy provisioning.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"const\": \"gateway.kgateway.dev/v1alpha1\",\n      \"description\": \"API version for the GatewayParameters resource.\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"GatewayParameters\",\n      \"description\": \"Resource kind.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Standard Kubernetes object metadata.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name\
  \ of the GatewayParameters resource.\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Namespace of the GatewayParameters resource.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"GatewayParametersSpec defines the desired state of GatewayParameters.\",\n      \"properties\": {\n        \"kube\": {\n          \"type\": \"object\",\n          \"description\": \"Kubernetes deployment settings.\",\n          \"properties\": {\n            \"deployment\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"replicas\": {\n                  \"type\": \"integer\"\
  ,\n                  \"description\": \"Number of gateway proxy replicas.\"\n                }\n              }\n            },\n            \"podTemplate\": {\n              \"type\": \"object\",\n              \"description\": \"Pod template configuration.\",\n              \"properties\": {\n                \"extraLabels\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": { \"type\": \"string\" }\n                },\n                \"extraAnnotations\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": { \"type\": \"string\" }\n                },\n                \"nodeSelector\": {\n                  \"type\": \"object\",\n                  \"additionalProperties\": { \"type\": \"string\" }\n                },\n                \"tolerations\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n      \
  \                \"key\": { \"type\": \"string\" },\n                      \"operator\": { \"type\": \"string\" },\n                      \"value\": { \"type\": \"string\" },\n                      \"effect\": { \"type\": \"string\" }\n                    }\n                  }\n                }\n              }\n            },\n            \"envoyContainer\": {\n              \"type\": \"object\",\n              \"description\": \"Envoy proxy container configuration.\",\n              \"properties\": {\n                \"resources\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"requests\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"cpu\": { \"type\": \"string\" },\n                        \"memory\": { \"type\": \"string\" }\n                      }\n                    },\n                    \"limits\": {\n                      \"type\": \"object\",\n  \
  \                    \"properties\": {\n                        \"cpu\": { \"type\": \"string\" },\n                        \"memory\": { \"type\": \"string\" }\n                      }\n                    }\n                  }\n                },\n                \"image\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"registry\": { \"type\": \"string\" },\n                    \"repository\": { \"type\": \"string\" },\n                    \"tag\": { \"type\": \"string\" }\n                  }\n                }\n              }\n            },\n            \"service\": {\n              \"type\": \"object\",\n              \"description\": \"Service configuration.\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"ClusterIP\", \"NodePort\", \"LoadBalancer\"]\n                },\n                \"extraAnnotations\": {\n                  \"type\"\
  : \"object\",\n                  \"additionalProperties\": { \"type\": \"string\" }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kgateway/refs/heads/main/json-schema/gateway-parameters.json
tags:
- Gateways
title: kgateway GatewayParameters
---
