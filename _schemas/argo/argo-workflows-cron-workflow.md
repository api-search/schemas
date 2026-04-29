---
description: A scheduled workflow resource
layout: schema
name: CronWorkflow
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-cron-workflow-schema.json
slug: argo-workflows-cron-workflow
source_filename: argo-workflows-cron-workflow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-schema.json\",\n  \"title\": \"CronWorkflow\",\n  \"description\": \"A scheduled workflow resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"default\": \"argoproj.io/v1alpha1\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"default\": \"CronWorkflow\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/components/schemas/ObjectMeta\"\n    },\n    \"spec\": {\n      \"$ref\": \"#/components/schemas/CronWorkflowSpec\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/CronWorkflowStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-cron-workflow-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: CronWorkflow
---
