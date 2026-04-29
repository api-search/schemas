---
description: ''
layout: schema
name: CreateMessageRequest
properties_list:
- description: The model that will complete your prompt. See the list of available models.
  name: model
  type: string
- description: The maximum number of tokens to generate before stopping. Different models support different maximum values.
  name: max_tokens
  type: integer
- description: Input messages. Alternating user and assistant conversational turns. Maximum 100,000 messages per request.
  name: messages
  type: array
- description: System prompt providing context and instructions to Claude. Can be a string or array of content blocks.
  name: system
  type: string
- description: Amount of randomness injected into the response. Ranges from 0.0 to 1.0. Use closer to 0.0 for analytical tasks, closer to 1.0 for creative tasks.
  name: temperature
  type: number
- description: Use nucleus sampling. Recommended to use either temperature or top_p, but not both.
  name: top_p
  type: number
- description: Only sample from the top K options for each subsequent token.
  name: top_k
  type: integer
- description: Custom text sequences that will cause the model to stop generating.
  name: stop_sequences
  type: array
- description: Whether to incrementally stream the response using server-sent events.
  name: stream
  type: boolean
- description: Definitions of tools that the model may use.
  name: tools
  type: array
- description: Service tier to use for this request.
  name: service_tier
  type: string
provider_name: Claude
provider_slug: claude
schema_file: json-schema/claude-messages-create-message-request-schema.json
slug: claude-messages-create-message-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateMessageRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model that will complete your prompt. See the list of available models.\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of tokens to generate before stopping. Different models support different maximum values.\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"Input messages. Alternating user and assistant conversational turns. Maximum 100,000 messages per request.\"\n    },\n    \"system\": {\n      \"type\": \"string\",\n      \"description\": \"System prompt providing context and instructions to Claude. Can be a string or array of content blocks.\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Amount of randomness\
  \ injected into the response. Ranges from 0.0 to 1.0. Use closer to 0.0 for analytical tasks, closer to 1.0 for creative tasks.\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"Use nucleus sampling. Recommended to use either temperature or top_p, but not both.\"\n    },\n    \"top_k\": {\n      \"type\": \"integer\",\n      \"description\": \"Only sample from the top K options for each subsequent token.\"\n    },\n    \"stop_sequences\": {\n      \"type\": \"array\",\n      \"description\": \"Custom text sequences that will cause the model to stop generating.\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to incrementally stream the response using server-sent events.\"\n    },\n    \"tools\": {\n      \"type\": \"array\",\n      \"description\": \"Definitions of tools that the model may use.\"\n    },\n    \"service_tier\": {\n      \"type\": \"string\",\n      \"description\": \"Service tier to use for this\
  \ request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/claude/refs/heads/main/json-schema/claude-messages-create-message-request-schema.json
tags:
- Artificial Intelligence
- Chatbot
- Conversational AI
- Generative AI
- Large Language Models
- Machine Learning
- Natural Language Processing
title: CreateMessageRequest
---
