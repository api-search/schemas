---
description: A PeerAuthentication defines how traffic will be tunneled (or not) to the sidecar proxy. It configures mutual TLS (mTLS) mode for workload-to-workload communication within the mesh.
layout: schema
name: Istio PeerAuthentication
properties_list:
- description: Workload selector to apply the policy to specific workloads. If not set, the policy applies to all workloads in the namespace.
  name: selector
  type: object
- description: Mutual TLS settings for workload communication.
  name: mtls
  type: object
- description: Port-specific mutual TLS settings. Keys are port numbers.
  name: portLevelMtls
  type: object
provider_name: Istio
provider_slug: istio
schema_file: json-schema/peer-authentication.json
slug: peer-authentication
source_filename: peer-authentication.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/istio/blob/main/json-schema/peer-authentication.json\",\n  \"title\": \"Istio PeerAuthentication\",\n  \"description\": \"A PeerAuthentication defines how traffic will be tunneled (or not) to the sidecar proxy. It configures mutual TLS (mTLS) mode for workload-to-workload communication within the mesh.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"selector\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"matchLabels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"One or more labels that indicate a specific set of pods/VMs on which the policy should be applied.\"\n        }\n      },\n      \"description\": \"Workload selector to apply the policy to specific workloads. If not set, the policy applies to all workloads in the namespace.\"\
  \n    },\n    \"mtls\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"mode\": {\n          \"type\": \"string\",\n          \"enum\": [\"UNSET\", \"DISABLE\", \"PERMISSIVE\", \"STRICT\"],\n          \"description\": \"Defines the mTLS mode used for peer authentication. UNSET inherits from parent, DISABLE disables mTLS tunnel, PERMISSIVE accepts both plaintext and mTLS, STRICT requires mTLS.\"\n        }\n      },\n      \"description\": \"Mutual TLS settings for workload communication.\"\n    },\n    \"portLevelMtls\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"mode\": {\n            \"type\": \"string\",\n            \"enum\": [\"UNSET\", \"DISABLE\", \"PERMISSIVE\", \"STRICT\"],\n            \"description\": \"Defines the mTLS mode for this specific port.\"\n          }\n        }\n      },\n      \"description\": \"Port-specific mutual TLS settings. Keys are port numbers.\"\
  \n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/istio/refs/heads/main/json-schema/peer-authentication.json
tags:
- CNCF
- Kubernetes
- Microservices
- Open Source
- Service Mesh
title: Istio PeerAuthentication
---
