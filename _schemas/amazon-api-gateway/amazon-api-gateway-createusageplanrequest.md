---
description: ''
layout: schema
name: CreateUsagePlanRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: apiStages
  type: array
- description: ''
  name: throttle
  type: object
- description: ''
  name: quota
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createusageplanrequest-schema.json
slug: amazon-api-gateway-createusageplanrequest
source_filename: amazon-api-gateway-createusageplanrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateUsagePlanRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"apiStages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ApiStage\"\n      }\n    },\n    \"throttle\": {\n      \"$ref\": \"#/definitions/ThrottleSettings\"\n    },\n    \"quota\": {\n      \"$ref\": \"#/definitions/QuotaSettings\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createusageplanrequest-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateUsagePlanRequest
---
