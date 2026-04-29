---
description: ''
layout: schema
name: ThrottleSettings
properties_list:
- description: The API request burst limit per second.
  name: burstLimit
  type: integer
- description: The API request steady-state rate limit per second.
  name: rateLimit
  type: number
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-throttlesettings-schema.json
slug: amazon-api-gateway-throttlesettings
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ThrottleSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"burstLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"The API request burst limit per second.\"\n    },\n    \"rateLimit\": {\n      \"type\": \"number\",\n      \"description\": \"The API request steady-state rate limit per second.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-throttlesettings-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: ThrottleSettings
---
