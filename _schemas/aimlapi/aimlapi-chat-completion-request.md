---
description: Request body for creating a chat completion via AIMLAPI
layout: schema
name: ChatCompletionRequest
properties_list:
- description: Model ID to use for completion
  name: model
  type: string
- description: List of messages in the conversation
  name: messages
  type: array
- description: Sampling temperature 0-2
  name: temperature
  type: number
- description: Maximum tokens to generate
  name: max_tokens
  type: integer
- description: Stream response tokens
  name: stream
  type: boolean
- description: Nucleus sampling parameter
  name: top_p
  type: number
- description: Frequency penalty -2 to 2
  name: frequency_penalty
  type: number
- description: Presence penalty -2 to 2
  name: presence_penalty
  type: number
provider_name: AIMLAPI
provider_slug: aimlapi
schema_file: json-schema/aimlapi-chat-completion-request-schema.json
slug: aimlapi-chat-completion-request
source_filename: aimlapi-chat-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-chat-completion-request-schema.json\",\n  \"title\": \"ChatCompletionRequest\",\n  \"description\": \"Request body for creating a chat completion via AIMLAPI\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model ID to use for completion\",\n      \"example\": \"gpt-4o\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"List of messages in the conversation\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Sampling temperature 0-2\",\n      \"example\": 0.7\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum tokens to generate\",\n      \"example\": 1024\n   \
  \ },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Stream response tokens\",\n      \"example\": false\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"Nucleus sampling parameter\",\n      \"example\": 1.0\n    },\n    \"frequency_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Frequency penalty -2 to 2\",\n      \"example\": 0\n    },\n    \"presence_penalty\": {\n      \"type\": \"number\",\n      \"description\": \"Presence penalty -2 to 2\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-chat-completion-request-schema.json
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
title: ChatCompletionRequest
---
