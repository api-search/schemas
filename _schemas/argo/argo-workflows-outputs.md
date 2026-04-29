---
description: Outputs from a template
layout: schema
name: Outputs
properties_list:
- description: ''
  name: parameters
  type: array
- description: ''
  name: artifacts
  type: array
- description: Result output from a script template
  name: result
  type: string
- description: Exit code of the container
  name: exitCode
  type: string
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-outputs-schema.json
slug: argo-workflows-outputs
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-outputs-schema.json\",\n  \"title\": \"Outputs\",\n  \"description\": \"Outputs from a template\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Parameter\"\n      }\n    },\n    \"artifacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Artifact\"\n      }\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"description\": \"Result output from a script template\"\n    },\n    \"exitCode\": {\n      \"type\": \"string\",\n      \"description\": \"Exit code of the container\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-outputs-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Outputs
---
