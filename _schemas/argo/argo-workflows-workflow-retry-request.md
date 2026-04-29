---
description: WorkflowRetryRequest schema from Argo API
layout: schema
name: WorkflowRetryRequest
properties_list:
- description: ''
  name: namespace
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: restartSuccessful
  type: boolean
- description: ''
  name: nodeFieldSelector
  type: string
- description: ''
  name: parameters
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-retry-request-schema.json
slug: argo-workflows-workflow-retry-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-retry-request-schema.json\",\n  \"title\": \"WorkflowRetryRequest\",\n  \"description\": \"WorkflowRetryRequest schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"restartSuccessful\": {\n      \"type\": \"boolean\"\n    },\n    \"nodeFieldSelector\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-retry-request-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowRetryRequest
---
