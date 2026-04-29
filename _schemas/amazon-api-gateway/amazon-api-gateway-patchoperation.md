---
description: ''
layout: schema
name: PatchOperation
properties_list:
- description: The operation type.
  name: op
  type: string
- description: The op operation's target, as identified by a JSON Pointer value.
  name: path
  type: string
- description: The new target value of the update operation. It is applicable for the add or replace operation.
  name: value
  type: string
- description: The copy update operation's source as identified by a JSON Pointer value.
  name: from
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-patchoperation-schema.json
slug: amazon-api-gateway-patchoperation
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"PatchOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"op\": {\n      \"type\": \"string\",\n      \"description\": \"The operation type.\",\n      \"enum\": [\n        \"add\",\n        \"remove\",\n        \"replace\",\n        \"move\",\n        \"copy\",\n        \"test\"\n      ]\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The op operation's target, as identified by a JSON Pointer value.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The new target value of the update operation. It is applicable for the add or replace operation.\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The copy update operation's source as identified by a JSON Pointer value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-patchoperation-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: PatchOperation
---
