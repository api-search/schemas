---
description: ''
layout: schema
name: PutMethodRequest
properties_list:
- description: The method's authorization type. Valid values are NONE, AWS_IAM, CUSTOM, or COGNITO_USER_POOLS.
  name: authorizationType
  type: string
- description: ''
  name: authorizerId
  type: string
- description: ''
  name: apiKeyRequired
  type: boolean
- description: ''
  name: operationName
  type: string
- description: ''
  name: requestParameters
  type: object
- description: ''
  name: requestModels
  type: object
- description: ''
  name: requestValidatorId
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-putmethodrequest-schema.json
slug: amazon-api-gateway-putmethodrequest
source_filename: amazon-api-gateway-putmethodrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"PutMethodRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizationType\": {\n      \"type\": \"string\",\n      \"description\": \"The method's authorization type. Valid values are NONE, AWS_IAM, CUSTOM, or COGNITO_USER_POOLS.\"\n    },\n    \"authorizerId\": {\n      \"type\": \"string\"\n    },\n    \"apiKeyRequired\": {\n      \"type\": \"boolean\"\n    },\n    \"operationName\": {\n      \"type\": \"string\"\n    },\n    \"requestParameters\": {\n      \"type\": \"object\"\n    },\n    \"requestModels\": {\n      \"type\": \"object\"\n    },\n    \"requestValidatorId\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"authorizationType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-putmethodrequest-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: PutMethodRequest
---
