---
description: PutMethodRequest schema from Amazon API Gateway v1 API
layout: schema
name: PutMethodRequest
properties_list:
- description: Authorization type (NONE, AWS_IAM, CUSTOM, COGNITO_USER_POOLS).
  name: authorizationType
  type: string
- description: Whether to require an API key.
  name: apiKeyRequired
  type: boolean
provider_name: Amazon API Gateway
provider_slug: aws-api-gateway
schema_file: json-schema/v1-put-method-request-schema.json
slug: v1-put-method-request
source_filename: v1-put-method-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizationType\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization type (NONE, AWS_IAM, CUSTOM, COGNITO_USER_POOLS).\",\n      \"example\": \"example-value\"\n    },\n    \"apiKeyRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to require an API key.\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"authorizationType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-put-method-request-schema.json\",\n  \"title\": \"PutMethodRequest\",\n  \"description\": \"PutMethodRequest schema from Amazon API Gateway v1 API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-api-gateway/refs/heads/main/json-schema/v1-put-method-request-schema.json
tags:
- API Gateway
- Cloud
- REST
- WebSocket
- Serverless
title: PutMethodRequest
---
