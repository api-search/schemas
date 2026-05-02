---
description: ''
layout: schema
name: CompletionResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: object
  type: string
- description: ''
  name: created
  type: integer
- description: ''
  name: model
  type: string
- description: ''
  name: choices
  type: array
- description: ''
  name: usage
  type: object
provider_name: Microsoft Azure API Management
provider_slug: microsoft-azure-api-management
schema_file: json-schema/ai-gateway-completion-response-schema.json
slug: ai-gateway-completion-response
source_filename: ai-gateway-completion-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletionResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"cmpl-xyz789\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"example\": \"text_completion\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"example\": 1714000000\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"example\": \"gpt-4o\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"index\": {\n            \"type\": \"integer\",\n            \"example\": 0\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"example\": \"enterprise environments includes centralized governance and security.\"\n          },\n          \"finish_reason\": {\n            \"type\": \"string\",\n        \
  \    \"example\": \"stop\"\n          }\n        }\n      }\n    },\n    \"usage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prompt_tokens\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"completion_tokens\": {\n          \"type\": \"integer\",\n          \"example\": 15\n        },\n        \"total_tokens\": {\n          \"type\": \"integer\",\n          \"example\": 25\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/json-schema/ai-gateway-completion-response-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Enterprise
- Microsoft Azure
title: CompletionResponse
---
