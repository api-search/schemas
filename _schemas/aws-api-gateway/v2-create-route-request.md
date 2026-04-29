---
description: CreateRouteRequest schema from Amazon API Gateway v2 API
layout: schema
name: CreateRouteRequest
properties_list:
- description: Route key for the new route.
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
schema_file: json-schema/v2-create-route-request-schema.json
slug: v2-create-route-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RouteKey\": {\n      \"type\": \"string\",\n      \"description\": \"Route key for the new route.\",\n      \"example\": \"example-value\"\n    },\n    \"Target\": {\n      \"type\": \"string\",\n      \"description\": \"Integration target reference.\",\n      \"example\": \"example-value\"\n    },\n    \"AuthorizationType\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization type for the route.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"RouteKey\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-route-request-schema.json\",\n  \"title\": \"CreateRouteRequest\",\n  \"description\": \"CreateRouteRequest schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-route-request-schema.json
tags:
- API Gateway
- AWS
- Cloud
- REST
- WebSocket
- Serverless
title: CreateRouteRequest
---
