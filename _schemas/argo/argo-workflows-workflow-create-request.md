---
description: WorkflowCreateRequest schema from Argo API
layout: schema
name: WorkflowCreateRequest
properties_list:
- description: ''
  name: namespace
  type: string
- description: ''
  name: workflow
  type: object
- description: ''
  name: serverDryRun
  type: boolean
- description: ''
  name: createOptions
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-create-request-schema.json
slug: argo-workflows-workflow-create-request
source_filename: argo-workflows-workflow-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-create-request-schema.json\",\n  \"title\": \"WorkflowCreateRequest\",\n  \"description\": \"WorkflowCreateRequest schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"workflow\": {\n      \"$ref\": \"#/components/schemas/Workflow\"\n    },\n    \"serverDryRun\": {\n      \"type\": \"boolean\"\n    },\n    \"createOptions\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-create-request-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowCreateRequest
---
