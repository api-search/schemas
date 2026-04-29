---
description: ''
layout: schema
name: GatewayResponses
properties_list:
- description: ''
  name: position
  type: string
- description: ''
  name: item
  type: array
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-gatewayresponses-schema.json
slug: amazon-api-gateway-gatewayresponses
source_filename: amazon-api-gateway-gatewayresponses-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GatewayResponses\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"position\": {\n      \"type\": \"string\"\n    },\n    \"item\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/GatewayResponse\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-gatewayresponses-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: GatewayResponses
---
