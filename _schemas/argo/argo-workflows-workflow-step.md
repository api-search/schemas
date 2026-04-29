---
description: A step in a steps template
layout: schema
name: WorkflowStep
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: template
  type: string
- description: ''
  name: arguments
  type: object
- description: ''
  name: when
  type: string
- description: ''
  name: withItems
  type: array
- description: ''
  name: withParam
  type: string
- description: ''
  name: continueOn
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-step-schema.json
slug: argo-workflows-workflow-step
source_filename: argo-workflows-workflow-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-step-schema.json\",\n  \"title\": \"WorkflowStep\",\n  \"description\": \"A step in a steps template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"template\": {\n      \"type\": \"string\"\n    },\n    \"arguments\": {\n      \"$ref\": \"#/components/schemas/Arguments\"\n    },\n    \"when\": {\n      \"type\": \"string\"\n    },\n    \"withItems\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"withParam\": {\n      \"type\": \"string\"\n    },\n    \"continueOn\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"error\": {\n          \"type\": \"boolean\"\n        },\n        \"failed\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-step-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowStep
---
