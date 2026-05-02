---
description: ''
layout: schema
name: CompletionRequest
properties_list:
- description: ''
  name: prompt
  type: string
- description: ''
  name: max_tokens
  type: integer
- description: ''
  name: temperature
  type: number
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
schema_file: json-schema/ai-gateway-completion-request-schema.json
slug: ai-gateway-completion-request
source_filename: ai-gateway-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"example\": \"Explain the benefits of API management in\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"example\": 128\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"example\": 0.7\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/json-schema/ai-gateway-completion-request-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Enterprise
- Microsoft Azure
title: CompletionRequest
---
