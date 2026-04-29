---
description: Status of a workflow execution
layout: schema
name: WorkflowStatus
properties_list:
- description: ''
  name: phase
  type: string
- description: ''
  name: startedAt
  type: string
- description: ''
  name: finishedAt
  type: string
- description: Progress of the workflow (e.g. 2/4)
  name: progress
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: estimatedDuration
  type: integer
- description: ''
  name: nodes
  type: object
- description: ''
  name: conditions
  type: array
- description: ''
  name: outputs
  type: object
- description: ''
  name: storedTemplates
  type: object
- description: ''
  name: artifactRepositoryRef
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-status-schema.json
slug: argo-workflows-workflow-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-status-schema.json\",\n  \"title\": \"WorkflowStatus\",\n  \"description\": \"Status of a workflow execution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phase\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Running\",\n        \"Succeeded\",\n        \"Failed\",\n        \"Error\"\n      ]\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"finishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"progress\": {\n      \"type\": \"string\",\n      \"description\": \"Progress of the workflow (e.g. 2/4)\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"estimatedDuration\": {\n      \"type\": \"integer\"\n    },\n    \"nodes\": {\n \
  \     \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/NodeStatus\"\n      }\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\"\n          },\n          \"message\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"outputs\": {\n      \"$ref\": \"#/components/schemas/Outputs\"\n    },\n    \"storedTemplates\": {\n      \"type\": \"object\"\n    },\n    \"artifactRepositoryRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"configMap\": {\n          \"type\": \"string\"\n        },\n        \"key\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-status-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowStatus
---
