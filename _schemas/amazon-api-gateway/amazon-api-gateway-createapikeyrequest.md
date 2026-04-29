---
description: ''
layout: schema
name: CreateApiKeyRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: generateDistinctId
  type: boolean
- description: ''
  name: value
  type: string
- description: ''
  name: stageKeys
  type: array
- description: ''
  name: customerId
  type: string
- description: ''
  name: tags
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createapikeyrequest-schema.json
slug: amazon-api-gateway-createapikeyrequest
source_filename: amazon-api-gateway-createapikeyrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateApiKeyRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"generateDistinctId\": {\n      \"type\": \"boolean\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"stageKeys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/StageKey\"\n      }\n    },\n    \"customerId\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createapikeyrequest-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateApiKeyRequest
---
