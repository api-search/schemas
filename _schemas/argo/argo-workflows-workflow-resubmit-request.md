---
description: WorkflowResubmitRequest schema from Argo API
layout: schema
name: WorkflowResubmitRequest
properties_list:
- description: ''
  name: namespace
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: memoized
  type: boolean
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-resubmit-request-schema.json
slug: argo-workflows-workflow-resubmit-request
source_filename: argo-workflows-workflow-resubmit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-resubmit-request-schema.json\",\n  \"title\": \"WorkflowResubmitRequest\",\n  \"description\": \"WorkflowResubmitRequest schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"memoized\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-resubmit-request-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowResubmitRequest
---
