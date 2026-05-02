---
description: ''
layout: schema
name: MCPResponse
properties_list:
- description: ''
  name: jsonrpc
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: result
  type: object
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
schema_file: json-schema/ai-gateway-mcp-response-schema.json
slug: ai-gateway-mcp-response
source_filename: ai-gateway-mcp-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MCPResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jsonrpc\": {\n      \"type\": \"string\",\n      \"example\": \"2.0\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"result\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"content\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"text\"\n              },\n              \"text\": {\n                \"type\": \"string\",\n                \"example\": \"The weather in Seattle is 62F and partly cloudy.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/json-schema/ai-gateway-mcp-response-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Enterprise
- Microsoft Azure
title: MCPResponse
---
