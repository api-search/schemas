---
description: Schema for a /chat/completions response from CometAPI (OpenAI-compatible).
layout: schema
name: CometAPI Chat Completion Response
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: object
  type: string
- description: ''
  name: model
  type: string
- description: Unix timestamp.
  name: created
  type: integer
- description: ''
  name: choices
  type: array
- description: ''
  name: usage
  type: object
provider_name: CometAPI
provider_slug: cometapi
schema_file: json-schema/cometapi-chat-completion-schema.json
slug: cometapi-chat-completion
source_filename: cometapi-chat-completion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/json-schema/cometapi-chat-completion-schema.json\",\n  \"title\": \"CometAPI Chat Completion Response\",\n  \"description\": \"Schema for a /chat/completions response from CometAPI (OpenAI-compatible).\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"model\", \"choices\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"chat.completion\"\n    },\n    \"model\": { \"type\": \"string\" },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp.\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"index\": { \"type\": \"integer\" },\n          \"message\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"role\": { \"type\": \"string\" },\n              \"content\": { \"type\": \"string\" }\n            }\n          },\n          \"finish_reason\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"usage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"prompt_tokens\": { \"type\": \"integer\" },\n        \"completion_tokens\": { \"type\": \"integer\" },\n        \"total_tokens\": { \"type\": \"integer\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cometapi/refs/heads/main/json-schema/cometapi-chat-completion-schema.json
tags:
- AI
- Aggregator
- Audio
- Chat
- Embeddings
- Generative AI
- Images
- LLM
- Multi-Model
- OpenAI-Compatible
- Video
title: CometAPI Chat Completion Response
---
