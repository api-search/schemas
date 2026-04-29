---
description: Arguments to pass to a template
layout: schema
name: Arguments
properties_list:
- description: ''
  name: parameters
  type: array
- description: ''
  name: artifacts
  type: array
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-arguments-schema.json
slug: argo-workflows-arguments
source_filename: argo-workflows-arguments-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-arguments-schema.json\",\n  \"title\": \"Arguments\",\n  \"description\": \"Arguments to pass to a template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Parameter\"\n      }\n    },\n    \"artifacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Artifact\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-arguments-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Arguments
---
