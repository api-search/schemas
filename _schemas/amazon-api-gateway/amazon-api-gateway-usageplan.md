---
description: ''
layout: schema
name: UsagePlan
properties_list:
- description: The identifier of the usage plan.
  name: id
  type: string
- description: The name of the usage plan.
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
  name: productCode
  type: string
- description: ''
  name: tags
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-usageplan-schema.json
slug: amazon-api-gateway-usageplan
source_filename: amazon-api-gateway-usageplan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"UsagePlan\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the usage plan.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the usage plan.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"apiStages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ApiStage\"\n      }\n    },\n    \"throttle\": {\n      \"$ref\": \"#/definitions/ThrottleSettings\"\n    },\n    \"quota\": {\n      \"$ref\": \"#/definitions/QuotaSettings\"\n    },\n    \"productCode\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-usageplan-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: UsagePlan
---
