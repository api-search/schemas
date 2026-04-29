---
description: WorkflowList schema from Argo API
layout: schema
name: WorkflowList
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: items
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-list-schema.json
slug: argo-workflows-workflow-list
source_filename: argo-workflows-workflow-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-list-schema.json\",\n  \"title\": \"WorkflowList\",\n  \"description\": \"WorkflowList schema from Argo API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"resourceVersion\": {\n          \"type\": \"string\"\n        },\n        \"continue\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Workflow\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-list-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowList
---
