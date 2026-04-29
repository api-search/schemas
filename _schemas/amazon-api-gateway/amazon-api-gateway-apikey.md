---
description: ''
layout: schema
name: ApiKey
properties_list:
- description: The identifier of the API key.
  name: id
  type: string
- description: The value of the API key.
  name: value
  type: string
- description: The name of the API key.
  name: name
  type: string
- description: An AWS Marketplace customer identifier.
  name: customerId
  type: string
- description: ''
  name: description
  type: string
- description: Whether the API key can be used by callers.
  name: enabled
  type: boolean
- description: ''
  name: createdDate
  type: string
- description: ''
  name: lastUpdatedDate
  type: string
- description: ''
  name: stageKeys
  type: array
- description: ''
  name: tags
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-apikey-schema.json
slug: amazon-api-gateway-apikey
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ApiKey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the API key.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the API key.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the API key.\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"An AWS Marketplace customer identifier.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the API key can be used by callers.\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"lastUpdatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"stageKeys\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-apikey-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: ApiKey
---
