---
description: ThrottleSettings schema from Amazon API Gateway v1 API
layout: schema
name: ThrottleSettings
properties_list:
- description: Burst limit for requests.
  name: burstLimit
  type: integer
- description: Steady-state rate limit (requests per second).
  name: rateLimit
  type: number
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-throttle-settings-schema.json
slug: v1-throttle-settings
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"burstLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Burst limit for requests.\",\n      \"example\": 49\n    },\n    \"rateLimit\": {\n      \"type\": \"number\",\n      \"description\": \"Steady-state rate limit (requests per second).\",\n      \"example\": 69.99\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-throttle-settings-schema.json\",\n  \"title\": \"ThrottleSettings\",\n  \"description\": \"ThrottleSettings schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-throttle-settings-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: ThrottleSettings
---
