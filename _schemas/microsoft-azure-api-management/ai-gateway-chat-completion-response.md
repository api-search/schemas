---
description: ''
layout: schema
name: ChatCompletionResponse
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
schema_file: json-schema/ai-gateway-chat-completion-response-schema.json
slug: ai-gateway-chat-completion-response
source_filename: ai-gateway-chat-completion-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"chatcmpl-abc123def456\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"example\": \"chat.completion\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"example\": 1714000000\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"example\": \"gpt-4o\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"index\": {\n            \"type\": \"integer\",\n            \"example\": 0\n          },\n          \"message\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"role\": {\n                \"type\": \"string\",\n                \"example\": \"assistant\"\n              },\n             \
  \ \"content\": {\n                \"type\": \"string\",\n                \"example\": \"Azure API Management is a hybrid, multicloud management platform for APIs across all environments.\"\n              }\n            }\n          },\n          \"finish_reason\": {\n            \"type\": \"string\",\n            \"example\": \"stop\"\n          }\n        }\n      }\n    },\n    \"usage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prompt_tokens\": {\n          \"type\": \"integer\",\n          \"example\": 24\n        },\n        \"completion_tokens\": {\n          \"type\": \"integer\",\n          \"example\": 18\n        },\n        \"total_tokens\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-api-management/refs/heads/main/json-schema/ai-gateway-chat-completion-response-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Enterprise
- Microsoft Azure
title: ChatCompletionResponse
---
