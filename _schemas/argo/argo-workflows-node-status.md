---
description: Status of a workflow node
layout: schema
name: NodeStatus
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: templateName
  type: string
- description: ''
  name: phase
  type: string
- description: ''
  name: startedAt
  type: string
- description: ''
  name: finishedAt
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: children
  type: array
- description: ''
  name: inputs
  type: object
- description: ''
  name: outputs
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-node-status-schema.json
slug: argo-workflows-node-status
source_filename: argo-workflows-node-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-node-status-schema.json\",\n  \"title\": \"NodeStatus\",\n  \"description\": \"Status of a workflow node\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pod\",\n        \"Steps\",\n        \"StepGroup\",\n        \"DAG\",\n        \"TaskGroup\",\n        \"Retry\",\n        \"Skipped\",\n        \"Suspend\"\n      ]\n    },\n    \"templateName\": {\n      \"type\": \"string\"\n    },\n    \"phase\": {\n      \"type\": \"string\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"finishedAt\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"inputs\": {\n      \"$ref\": \"#/components/schemas/Inputs\"\n    },\n    \"outputs\": {\n      \"$ref\": \"#/components/schemas/Outputs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-node-status-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: NodeStatus
---
