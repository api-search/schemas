---
description: A Node Template defines instance type constraints and configuration for nodes provisioned by the CAST AI autoscaler.
layout: schema
name: CAST AI Node Template
properties_list:
- description: Unique identifier for the node template.
  name: id
  type: string
- description: Name of the node template.
  name: name
  type: string
- description: ID of the associated node configuration.
  name: configurationId
  type: string
- description: Resource constraints for node selection.
  name: constraints
  type: object
- description: Timestamp when the node template was created.
  name: createdAt
  type: string
- description: Timestamp when the node template was last updated.
  name: updatedAt
  type: string
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/node-template.json
slug: node-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cast-ai/blob/main/json-schema/node-template.json\",\n  \"title\": \"CAST AI Node Template\",\n  \"description\": \"A Node Template defines instance type constraints and configuration for nodes provisioned by the CAST AI autoscaler.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the node template.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the node template.\"\n    },\n    \"configurationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the associated node configuration.\"\n    },\n    \"constraints\": {\n      \"type\": \"object\",\n      \"description\": \"Resource constraints for node selection.\",\n      \"properties\": {\n        \"minCpu\":\
  \ {\n          \"type\": \"integer\",\n          \"description\": \"Minimum number of CPUs for the node.\"\n        },\n        \"maxCpu\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of CPUs for the node.\"\n        },\n        \"minMemory\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum memory in MiB for the node.\"\n        },\n        \"maxMemory\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum memory in MiB for the node.\"\n        },\n        \"useSpotInstances\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to use spot or preemptible instances.\"\n        },\n        \"architectures\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Allowed CPU architectures (e.g., amd64, arm64).\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Timestamp when the node template was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the node template was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/json-schema/node-template.json
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Node Template
---
