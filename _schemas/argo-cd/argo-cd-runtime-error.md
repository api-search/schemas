---
description: runtimeError schema from Argo CD API
layout: schema
name: runtimeError
properties_list:
- description: ''
  name: code
  type: integer
- description: ''
  name: details
  type: array
- description: ''
  name: error
  type: string
- description: ''
  name: message
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-runtime-error-schema.json
slug: argo-cd-runtime-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-runtime-error-schema.json\",\n  \"title\": \"runtimeError\",\n  \"description\": \"runtimeError schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/protobufAny\"\n      }\n    },\n    \"error\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-runtime-error-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: runtimeError
---
