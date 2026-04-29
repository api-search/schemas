---
description: grpc.gateway.runtime.StreamError schema from Argo Workflows API
layout: schema
name: grpc.gateway.runtime.StreamError
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
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-grpc-gateway-runtime-stream-error-schema.json
slug: argo-workflows-grpc-gateway-runtime-stream-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-grpc-gateway-runtime-stream-error-schema.json\",\n  \"title\": \"grpc.gateway.runtime.StreamError\",\n  \"description\": \"grpc.gateway.runtime.StreamError schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"details\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/google.protobuf.Any\"\n      }\n    },\n    \"grpc_code\": {\n      \"type\": \"integer\"\n    },\n    \"http_code\": {\n      \"type\": \"integer\"\n    },\n    \"http_status\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-grpc-gateway-runtime-stream-error-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: grpc.gateway.runtime.StreamError
---
