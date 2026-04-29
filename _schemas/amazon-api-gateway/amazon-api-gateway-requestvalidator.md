---
description: ''
layout: schema
name: RequestValidator
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: validateRequestBody
  type: boolean
- description: ''
  name: validateRequestParameters
  type: boolean
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-requestvalidator-schema.json
slug: amazon-api-gateway-requestvalidator
source_filename: amazon-api-gateway-requestvalidator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"RequestValidator\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"validateRequestBody\": {\n      \"type\": \"boolean\"\n    },\n    \"validateRequestParameters\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-requestvalidator-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: RequestValidator
---
