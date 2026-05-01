---
description: ''
layout: schema
name: PutIntegrationRequest
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: httpMethod
  type: string
- description: ''
  name: uri
  type: string
- description: ''
  name: connectionType
  type: string
- description: ''
  name: connectionId
  type: string
- description: ''
  name: credentials
  type: string
- description: ''
  name: requestParameters
  type: object
- description: ''
  name: requestTemplates
  type: object
- description: ''
  name: passthroughBehavior
  type: string
- description: ''
  name: contentHandling
  type: string
- description: ''
  name: timeoutInMillis
  type: integer
- description: ''
  name: cacheNamespace
  type: string
- description: ''
  name: cacheKeyParameters
  type: array
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-putintegrationrequest-schema.json
slug: amazon-api-gateway-putintegrationrequest
source_filename: amazon-api-gateway-putintegrationrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"PutIntegrationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HTTP\",\n        \"HTTP_PROXY\",\n        \"AWS\",\n        \"AWS_PROXY\",\n        \"MOCK\"\n      ]\n    },\n    \"httpMethod\": {\n      \"type\": \"string\"\n    },\n    \"uri\": {\n      \"type\": \"string\"\n    },\n    \"connectionType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INTERNET\",\n        \"VPC_LINK\"\n      ]\n    },\n    \"connectionId\": {\n      \"type\": \"string\"\n    },\n    \"credentials\": {\n      \"type\": \"string\"\n    },\n    \"requestParameters\": {\n      \"type\": \"object\"\n    },\n    \"requestTemplates\": {\n      \"type\": \"object\"\n    },\n    \"passthroughBehavior\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"WHEN_NO_MATCH\",\n        \"WHEN_NO_TEMPLATES\",\n        \"\
  NEVER\"\n      ]\n    },\n    \"contentHandling\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONVERT_TO_BINARY\",\n        \"CONVERT_TO_TEXT\"\n      ]\n    },\n    \"timeoutInMillis\": {\n      \"type\": \"integer\"\n    },\n    \"cacheNamespace\": {\n      \"type\": \"string\"\n    },\n    \"cacheKeyParameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-putintegrationrequest-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: PutIntegrationRequest
---
