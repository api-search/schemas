---
description: ''
layout: schema
name: ChatCompletionRequest
properties_list:
- description: Model identifier (can be tgi or a model ID)
  name: model
  type: string
- description: Conversation messages
  name: messages
  type: array
- description: ''
  name: frequency_penalty
  type: number
- description: ''
  name: logprobs
  type: boolean
- description: Maximum tokens to generate
  name: max_tokens
  type: integer
- description: ''
  name: presence_penalty
  type: number
- description: ''
  name: response_format
  type: string
- description: ''
  name: seed
  type: integer
- description: ''
  name: stop
  type: array
- description: ''
  name: stream
  type: boolean
- description: ''
  name: stream_options
  type: object
- description: ''
  name: temperature
  type: number
- description: ''
  name: tool_choice
  type: string
- description: Prompt appended before tools
  name: tool_prompt
  type: string
- description: ''
  name: tools
  type: array
- description: ''
  name: top_logprobs
  type: integer
- description: ''
  name: top_p
  type: number
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-text-generation-inference-chat-completion-request-schema.json
slug: hugging-face-text-generation-inference-chat-completion-request
source_filename: hugging-face-text-generation-inference-chat-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model identifier (can be tgi or a model ID)\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"Conversation messages\"\n    },\n    \"frequency_penalty\": {\n      \"type\": \"number\"\n    },\n    \"logprobs\": {\n      \"type\": \"boolean\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum tokens to generate\"\n    },\n    \"presence_penalty\": {\n      \"type\": \"number\"\n    },\n    \"response_format\": {\n      \"type\": \"string\"\n    },\n    \"seed\": {\n      \"type\": \"integer\"\n    },\n    \"stop\": {\n      \"type\": \"array\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\"\n    },\n    \"stream_options\": {\n      \"type\": \"object\"\n    },\n   \
  \ \"temperature\": {\n      \"type\": \"number\"\n    },\n    \"tool_choice\": {\n      \"type\": \"string\"\n    },\n    \"tool_prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Prompt appended before tools\"\n    },\n    \"tools\": {\n      \"type\": \"array\"\n    },\n    \"top_logprobs\": {\n      \"type\": \"integer\"\n    },\n    \"top_p\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-text-generation-inference-chat-completion-request-schema.json
tags: []
title: ChatCompletionRequest
---
