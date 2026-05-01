---
description: Method schema from Amazon API Gateway v1 API
layout: schema
name: Method
properties_list:
- description: HTTP method verb.
  name: httpMethod
  type: string
- description: Authorization type for invoking the method.
  name: authorizationType
  type: string
- description: Whether the method requires an API key.
  name: apiKeyRequired
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-method-schema.json
slug: v1-method
source_filename: v1-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"httpMethod\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP method verb.\",\n      \"example\": \"example-value\"\n    },\n    \"authorizationType\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization type for invoking the method.\",\n      \"example\": \"example-value\"\n    },\n    \"apiKeyRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the method requires an API key.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-method-schema.json\",\n  \"title\": \"Method\",\n  \"description\": \"Method schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-method-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: Method
---
