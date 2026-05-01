---
description: ''
layout: schema
name: Models
properties_list:
- description: ''
  name: position
  type: string
- description: ''
  name: item
  type: array
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-models-schema.json
slug: amazon-api-gateway-models
source_filename: amazon-api-gateway-models-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Models\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"position\": {\n      \"type\": \"string\"\n    },\n    \"item\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Model\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-models-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: Models
---
