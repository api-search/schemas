---
description: ''
layout: schema
name: Error
properties_list:
- description: A human-readable error message.
  name: message
  type: string
- description: The error code.
  name: code
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-error-schema.json
slug: amazon-api-gateway-error
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-error-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: Error
---
