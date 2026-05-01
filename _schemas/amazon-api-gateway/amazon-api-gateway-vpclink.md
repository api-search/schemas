---
description: ''
layout: schema
name: VpcLink
properties_list:
- description: ''
  name: id
  type: string
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
  name: status
  type: string
- description: ''
  name: statusMessage
  type: string
- description: ''
  name: tags
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-vpclink-schema.json
slug: amazon-api-gateway-vpclink
source_filename: amazon-api-gateway-vpclink-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VpcLink\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"targetArns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"PENDING\",\n        \"DELETING\",\n        \"FAILED\"\n      ]\n    },\n    \"statusMessage\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-vpclink-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: VpcLink
---
