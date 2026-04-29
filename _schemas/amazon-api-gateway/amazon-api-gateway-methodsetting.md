---
description: ''
layout: schema
name: MethodSetting
properties_list:
- description: ''
  name: metricsEnabled
  type: boolean
- description: ''
  name: loggingLevel
  type: string
- description: ''
  name: dataTraceEnabled
  type: boolean
- description: ''
  name: throttlingBurstLimit
  type: integer
- description: ''
  name: throttlingRateLimit
  type: number
- description: ''
  name: cachingEnabled
  type: boolean
- description: ''
  name: cacheTtlInSeconds
  type: integer
- description: ''
  name: cacheDataEncrypted
  type: boolean
- description: ''
  name: requireAuthorizationForCacheControl
  type: boolean
- description: ''
  name: unauthorizedCacheControlHeaderStrategy
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-methodsetting-schema.json
slug: amazon-api-gateway-methodsetting
source_filename: amazon-api-gateway-methodsetting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MethodSetting\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricsEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"loggingLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OFF\",\n        \"ERROR\",\n        \"INFO\"\n      ]\n    },\n    \"dataTraceEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"throttlingBurstLimit\": {\n      \"type\": \"integer\"\n    },\n    \"throttlingRateLimit\": {\n      \"type\": \"number\"\n    },\n    \"cachingEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"cacheTtlInSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"cacheDataEncrypted\": {\n      \"type\": \"boolean\"\n    },\n    \"requireAuthorizationForCacheControl\": {\n      \"type\": \"boolean\"\n    },\n    \"unauthorizedCacheControlHeaderStrategy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"FAIL_WITH_403\",\n        \"SUCCEED_WITH_RESPONSE_HEADER\"\
  ,\n        \"SUCCEED_WITHOUT_RESPONSE_HEADER\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-methodsetting-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: MethodSetting
---
