---
description: Response from a chat completion request
layout: schema
name: ChatCompletionResponse
properties_list:
- description: Unique completion ID
  name: id
  type: string
- description: Object type
  name: object
  type: string
- description: Model used for completion
  name: model
  type: string
- description: List of completion choices
  name: choices
  type: array
- description: Token usage statistics
  name: usage
  type: object
- description: Unix timestamp of creation
  name: created
  type: integer
provider_name: AIMLAPI
provider_slug: aimlapi
schema_file: json-schema/aimlapi-chat-completion-response-schema.json
slug: aimlapi-chat-completion-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-chat-completion-response-schema.json\",\n  \"title\": \"ChatCompletionResponse\",\n  \"description\": \"Response from a chat completion request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique completion ID\",\n      \"example\": \"chatcmpl-abc123\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"Object type\",\n      \"example\": \"chat.completion\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model used for completion\",\n      \"example\": \"gpt-4o\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"description\": \"List of completion choices\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"usage\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Token usage statistics\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of creation\",\n      \"example\": 1718153645\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-chat-completion-response-schema.json
tags:
- Artificial Intelligence
- Machine Learning
- AI Models
- LLM
- Image Generation
- Video Generation
- Speech
- Embeddings
- API Gateway
- Developer Tools
title: ChatCompletionResponse
---
