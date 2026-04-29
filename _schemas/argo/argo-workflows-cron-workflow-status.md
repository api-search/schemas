---
description: Status of a cron workflow
layout: schema
name: CronWorkflowStatus
properties_list:
- description: ''
  name: active
  type: array
- description: ''
  name: lastScheduledTime
  type: string
- description: ''
  name: conditions
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-cron-workflow-status-schema.json
slug: argo-workflows-cron-workflow-status
source_filename: argo-workflows-cron-workflow-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-status-schema.json\",\n  \"title\": \"CronWorkflowStatus\",\n  \"description\": \"Status of a cron workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"active\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"lastScheduledTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-status-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: CronWorkflowStatus
---
