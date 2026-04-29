---
description: ''
layout: schema
name: CreateAuthorizerRequest
properties_list:
- description: The name of the authorizer.
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: providerARNs
  type: array
- description: ''
  name: authType
  type: string
- description: ''
  name: authorizerUri
  type: string
- description: ''
  name: authorizerCredentials
  type: string
- description: ''
  name: identitySource
  type: string
- description: ''
  name: identityValidationExpression
  type: string
- description: ''
  name: authorizerResultTtlInSeconds
  type: integer
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createauthorizerrequest-schema.json
slug: amazon-api-gateway-createauthorizerrequest
source_filename: amazon-api-gateway-createauthorizerrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateAuthorizerRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the authorizer.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TOKEN\",\n        \"REQUEST\",\n        \"COGNITO_USER_POOLS\"\n      ]\n    },\n    \"providerARNs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"authType\": {\n      \"type\": \"string\"\n    },\n    \"authorizerUri\": {\n      \"type\": \"string\"\n    },\n    \"authorizerCredentials\": {\n      \"type\": \"string\"\n    },\n    \"identitySource\": {\n      \"type\": \"string\"\n    },\n    \"identityValidationExpression\": {\n      \"type\": \"string\"\n    },\n    \"authorizerResultTtlInSeconds\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"name\",\n  \
  \  \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createauthorizerrequest-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateAuthorizerRequest
---
