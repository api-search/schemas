---
description: ''
layout: schema
name: GatewayResponse
properties_list:
- description: ''
  name: responseType
  type: string
- description: ''
  name: statusCode
  type: string
- description: ''
  name: responseParameters
  type: object
- description: ''
  name: responseTemplates
  type: object
- description: ''
  name: defaultResponse
  type: boolean
provider_name: Amazon API Gateway
provider_slug: amazon-api-gateway
schema_file: json-schema/amazon-api-gateway-gatewayresponse-schema.json
slug: amazon-api-gateway-gatewayresponse
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GatewayResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"responseType\": {\n      \"type\": \"string\"\n    },\n    \"statusCode\": {\n      \"type\": \"string\"\n    },\n    \"responseParameters\": {\n      \"type\": \"object\"\n    },\n    \"responseTemplates\": {\n      \"type\": \"object\"\n    },\n    \"defaultResponse\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-api-gateway/refs/heads/main/json-schema/amazon-api-gateway-gatewayresponse-schema.json
tags:
- AWS
- Gateway
- HTTP API
- REST API
- Serverless
- WebSocket
title: GatewayResponse
---
