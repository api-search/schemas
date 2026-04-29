---
description: Request body for creating a chat completion.
layout: schema
name: ChatCompletionRequest
properties_list:
- description: Provider and model name in the format provider/model-name (e.g., openai/gpt-4o, anthropic/claude-3-5-sonnet-20241022).
  name: model
  type: string
- description: Array of messages comprising the conversation.
  name: messages
  type: array
- description: Sampling temperature between 0 and 2.
  name: temperature
  type: number
- description: Maximum number of tokens to generate.
  name: max_tokens
  type: integer
- description: Whether to stream the response as SSE.
  name: stream
  type: boolean
- description: Nucleus sampling probability.
  name: top_p
  type: number
- description: Number of completions to generate.
  name: n
  type: integer
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-chat-completion-request-schema.json
slug: bifrost-chat-completion-request
source_filename: bifrost-chat-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ChatCompletionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a chat completion.\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Provider and model name in the format provider/model-name (e.g., openai/gpt-4o, anthropic/claude-3-5-sonnet-20241022).\",\n      \"example\": \"openai/gpt-4o\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"Array of messages comprising the conversation.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ChatMessage\"\n      }\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Sampling temperature between 0 and 2.\",\n      \"example\": 0.7\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of tokens to generate.\",\n      \"example\": 256\n    },\n   \
  \ \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to stream the response as SSE.\",\n      \"example\": false\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"Nucleus sampling probability.\",\n      \"example\": 1.0\n    },\n    \"n\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of completions to generate.\",\n      \"example\": 1\n    }\n  },\n  \"required\": [\n    \"model\",\n    \"messages\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/json-schema/bifrost-chat-completion-request-schema.json
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: ChatCompletionRequest
---
