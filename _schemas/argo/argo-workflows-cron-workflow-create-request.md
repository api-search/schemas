---
description: CronWorkflowCreateRequest schema from Argo API
layout: schema
name: CronWorkflowCreateRequest
properties_list:
- description: ''
  name: namespace
  type: string
- description: ''
  name: cronWorkflow
  type: object
- description: ''
  name: createOptions
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-cron-workflow-create-request-schema.json
slug: argo-workflows-cron-workflow-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-create-request-schema.json\",\n  \"title\": \"CronWorkflowCreateRequest\",\n  \"description\": \"CronWorkflowCreateRequest schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\"\n    },\n    \"cronWorkflow\": {\n      \"$ref\": \"#/components/schemas/CronWorkflow\"\n    },\n    \"createOptions\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-create-request-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: CronWorkflowCreateRequest
---
