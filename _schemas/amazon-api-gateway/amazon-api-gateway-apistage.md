---
description: ''
layout: schema
name: ApiStage
properties_list:
- description: ''
  name: apiId
  type: string
- description: ''
  name: stage
  type: string
- description: ''
  name: throttle
  type: object
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-apistage-schema.json
slug: amazon-api-gateway-apistage
source_filename: amazon-api-gateway-apistage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ApiStage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiId\": {\n      \"type\": \"string\"\n    },\n    \"stage\": {\n      \"type\": \"string\"\n    },\n    \"throttle\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-apistage-schema.json
tags:
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: ApiStage
---
