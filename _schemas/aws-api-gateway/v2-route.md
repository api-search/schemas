---
description: Route schema from Amazon API Gateway v2 API
layout: schema
name: Route
properties_list:
- description: Route identifier.
  name: RouteId
  type: string
- description: Route key (e.g. "GET /items" or "$connect").
  name: RouteKey
  type: string
- description: Integration target reference.
  name: Target
  type: string
- description: Authorization type for the route.
  name: AuthorizationType
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-route-schema.json
slug: v2-route
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RouteId\": {\n      \"type\": \"string\",\n      \"description\": \"Route identifier.\",\n      \"example\": \"abc123\"\n    },\n    \"RouteKey\": {\n      \"type\": \"string\",\n      \"description\": \"Route key (e.g. \\\"GET /items\\\" or \\\"$connect\\\").\",\n      \"example\": \"example-value\"\n    },\n    \"Target\": {\n      \"type\": \"string\",\n      \"description\": \"Integration target reference.\",\n      \"example\": \"example-value\"\n    },\n    \"AuthorizationType\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization type for the route.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-route-schema.json\",\n  \"title\": \"Route\",\n  \"description\": \"Route schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-route-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: Route
---
