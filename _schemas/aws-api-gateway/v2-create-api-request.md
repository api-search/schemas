---
description: CreateApiRequest schema from Amazon API Gateway v2 API
layout: schema
name: CreateApiRequest
properties_list:
- description: Name of the API.
  name: Name
  type: string
- description: Protocol type for the API.
  name: ProtocolType
  type: string
- description: Route selection expression (required for WebSocket APIs).
  name: RouteSelectionExpression
  type: string
- description: Description of the API.
  name: Description
  type: string
- description: Quick-create target Lambda or HTTP endpoint URI.
  name: Target
  type: string
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v2-create-api-request-schema.json
slug: v2-create-api-request
source_filename: v2-create-api-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the API.\",\n      \"example\": \"my-resource\"\n    },\n    \"ProtocolType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HTTP\",\n        \"WEBSOCKET\"\n      ],\n      \"description\": \"Protocol type for the API.\",\n      \"example\": \"HTTP\"\n    },\n    \"RouteSelectionExpression\": {\n      \"type\": \"string\",\n      \"description\": \"Route selection expression (required for WebSocket APIs).\",\n      \"example\": \"example-value\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API.\",\n      \"example\": \"A description of this resource.\"\n    },\n    \"Target\": {\n      \"type\": \"string\",\n      \"description\": \"Quick-create target Lambda or HTTP endpoint URI.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"\
  ProtocolType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-api-request-schema.json\",\n  \"title\": \"CreateApiRequest\",\n  \"description\": \"CreateApiRequest schema from Amazon API Gateway v2 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v2-create-api-request-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: CreateApiRequest
---
