---
description: ''
layout: schema
name: CreateVpcLinkRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: targetArns
  type: array
- description: ''
  name: tags
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-createvpclinkrequest-schema.json
slug: amazon-api-gateway-createvpclinkrequest
source_filename: amazon-api-gateway-createvpclinkrequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateVpcLinkRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"targetArns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"targetArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-createvpclinkrequest-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: CreateVpcLinkRequest
---
