---
description: CronWorkflowUpdateRequest schema from Argo API
layout: schema
name: CronWorkflowUpdateRequest
properties_list:
- description: ''
  name: namespace
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: cronWorkflow
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-cron-workflow-update-request-schema.json
slug: argo-workflows-cron-workflow-update-request
source_filename: argo-workflows-cron-workflow-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-update-request-schema.json\",\n  \"title\": \"CronWorkflowUpdateRequest\",\n  \"description\": \"CronWorkflowUpdateRequest schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"cronWorkflow\": {\n      \"$ref\": \"#/components/schemas/CronWorkflow\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-update-request-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: CronWorkflowUpdateRequest
---
