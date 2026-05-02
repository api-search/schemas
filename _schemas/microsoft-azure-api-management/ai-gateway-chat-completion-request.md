---
description: ''
layout: schema
name: ChatCompletionRequest
properties_list:
- description: ''
  name: messages
  type: array
- description: ''
  name: max_tokens
  type: integer
- description: ''
  name: temperature
  type: number
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
schema_file: json-schema/ai-gateway-chat-completion-request-schema.json
slug: ai-gateway-chat-completion-request
source_filename: ai-gateway-chat-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"role\": {\n            \"type\": \"string\",\n            \"example\": \"user\"\n          },\n          \"content\": {\n            \"type\": \"string\",\n            \"example\": \"What is Azure API Management?\"\n          }\n        }\n      }\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"example\": 256\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"example\": 0.7\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/json-schema/ai-gateway-chat-completion-request-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Enterprise
- Microsoft Azure
title: ChatCompletionRequest
---
