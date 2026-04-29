---
description: Inputs for a template
layout: schema
name: Inputs
properties_list:
- description: ''
  name: parameters
  type: array
- description: ''
  name: artifacts
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-inputs-schema.json
slug: argo-workflows-inputs
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-inputs-schema.json\",\n  \"title\": \"Inputs\",\n  \"description\": \"Inputs for a template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Parameter\"\n      }\n    },\n    \"artifacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Artifact\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-inputs-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Inputs
---
