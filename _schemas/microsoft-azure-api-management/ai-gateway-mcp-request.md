---
description: ''
layout: schema
name: MCPRequest
properties_list:
- description: ''
  name: jsonrpc
  type: string
- description: ''
  name: method
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: params
  type: object
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
schema_file: json-schema/ai-gateway-mcp-request-schema.json
slug: ai-gateway-mcp-request
source_filename: ai-gateway-mcp-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MCPRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jsonrpc\": {\n      \"type\": \"string\",\n      \"example\": \"2.0\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"example\": \"tools/call\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"params\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"get_weather\"\n        },\n        \"arguments\": {\n          \"type\": \"object\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/json-schema/ai-gateway-mcp-request-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Enterprise
- Microsoft Azure
title: MCPRequest
---
