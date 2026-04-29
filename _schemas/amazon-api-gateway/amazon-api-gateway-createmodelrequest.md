---
description: ''
layout: schema
name: CreateModelRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: schema
  type: string
- description: ''
  name: contentType
  type: string
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createmodelrequest-schema.json
slug: amazon-api-gateway-createmodelrequest
source_filename: amazon-api-gateway-createmodelrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateModelRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"schema\": {\n      \"type\": \"string\"\n    },\n    \"contentType\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"contentType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createmodelrequest-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateModelRequest
---
