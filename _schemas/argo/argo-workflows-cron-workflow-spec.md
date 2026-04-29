---
description: Specification of a cron workflow
layout: schema
name: CronWorkflowSpec
properties_list:
- description: Cron schedule expression
  name: schedule
  type: string
- description: Timezone for the cron schedule
  name: timezone
  type: string
- description: ''
  name: startingDeadlineSeconds
  type: integer
- description: ''
  name: concurrencyPolicy
  type: string
- description: Whether the cron workflow is suspended
  name: suspend
  type: boolean
- description: ''
  name: successfulJobsHistoryLimit
  type: integer
- description: ''
  name: failedJobsHistoryLimit
  type: integer
- description: ''
  name: workflowSpec
  type: object
- description: ''
  name: workflowMetadata
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-cron-workflow-spec-schema.json
slug: argo-workflows-cron-workflow-spec
source_filename: argo-workflows-cron-workflow-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-spec-schema.json\",\n  \"title\": \"CronWorkflowSpec\",\n  \"description\": \"Specification of a cron workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schedule\": {\n      \"type\": \"string\",\n      \"description\": \"Cron schedule expression\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for the cron schedule\"\n    },\n    \"startingDeadlineSeconds\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"concurrencyPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Allow\",\n        \"Forbid\",\n        \"Replace\"\n      ]\n    },\n    \"suspend\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cron workflow is suspended\"\n    },\n    \"successfulJobsHistoryLimit\"\
  : {\n      \"type\": \"integer\"\n    },\n    \"failedJobsHistoryLimit\": {\n      \"type\": \"integer\"\n    },\n    \"workflowSpec\": {\n      \"$ref\": \"#/components/schemas/WorkflowSpec\"\n    },\n    \"workflowMetadata\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-spec-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: CronWorkflowSpec
---
