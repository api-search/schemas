---
description: Apis schema from Amazon API Gateway v2 API
layout: schema
name: Apis
properties_list:
- description: ''
  name: Items
  type: array
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-apis-schema.json
slug: v2-apis
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ApiId\": {\n            \"type\": \"string\",\n            \"description\": \"Identifier of the API.\",\n            \"example\": \"abc123\"\n          },\n          \"Name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the API.\",\n            \"example\": \"my-resource\"\n          },\n          \"ProtocolType\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HTTP\",\n              \"WEBSOCKET\"\n            ],\n            \"description\": \"API protocol (HTTP or WEBSOCKET).\",\n            \"example\": \"HTTP\"\n          },\n          \"ApiEndpoint\": {\n            \"type\": \"string\",\n            \"description\": \"Default endpoint for the API.\",\n            \"example\": \"example-value\"\n          },\n          \"RouteSelectionExpression\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"Route selection expression for the API.\",\n            \"example\": \"example-value\"\n          },\n          \"CreatedDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp when the API was created.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        }\n      },\n      \"example\": [\n        \"example-value\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-apis-schema.json\",\n  \"title\": \"Apis\",\n  \"description\": \"Apis schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-apis-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Apis
---
