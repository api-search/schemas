---
description: ''
layout: schema
name: DocumentationVersions
properties_list:
- description: ''
  name: position
  type: string
- description: ''
  name: item
  type: array
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-documentationversions-schema.json
slug: amazon-api-gateway-documentationversions
source_filename: amazon-api-gateway-documentationversions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DocumentationVersions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"position\": {\n      \"type\": \"string\"\n    },\n    \"item\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/DocumentationVersion\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-documentationversions-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: DocumentationVersions
---
