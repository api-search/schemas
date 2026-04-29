---
description: runtimeStreamError schema from Argo CD API
layout: schema
name: runtimeStreamError
properties_list:
- description: ''
  name: details
  type: array
- description: ''
  name: grpc_code
  type: integer
- description: ''
  name: http_code
  type: integer
- description: ''
  name: http_status
  type: string
- description: ''
  name: message
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-runtime-stream-error-schema.json
slug: argo-cd-runtime-stream-error
source_filename: argo-cd-runtime-stream-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-runtime-stream-error-schema.json\",\n  \"title\": \"runtimeStreamError\",\n  \"description\": \"runtimeStreamError schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"details\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/protobufAny\"\n      }\n    },\n    \"grpc_code\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"http_code\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"http_status\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-runtime-stream-error-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: runtimeStreamError
---
