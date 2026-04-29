---
description: grpc.gateway.runtime.Error schema from Argo Workflows API
layout: schema
name: grpc.gateway.runtime.Error
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
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-grpc-gateway-runtime-error-schema.json
slug: argo-workflows-grpc-gateway-runtime-error
source_filename: argo-workflows-grpc-gateway-runtime-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-grpc-gateway-runtime-error-schema.json\",\n  \"title\": \"grpc.gateway.runtime.Error\",\n  \"description\": \"grpc.gateway.runtime.Error schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\"\n    },\n    \"details\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/google.protobuf.Any\"\n      }\n    },\n    \"error\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-grpc-gateway-runtime-error-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: grpc.gateway.runtime.Error
---
