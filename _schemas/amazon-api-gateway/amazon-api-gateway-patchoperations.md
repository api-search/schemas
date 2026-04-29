---
description: ''
layout: schema
name: PatchOperations
properties_list:
- description: ''
  name: patchOperations
  type: array
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-patchoperations-schema.json
slug: amazon-api-gateway-patchoperations
source_filename: amazon-api-gateway-patchoperations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"PatchOperations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"patchOperations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/PatchOperation\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-patchoperations-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: PatchOperations
---
