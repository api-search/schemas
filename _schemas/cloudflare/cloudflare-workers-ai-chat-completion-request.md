---
description: ''
layout: schema
name: ChatCompletionRequest
properties_list:
- description: The model identifier, e.g. @cf/meta/llama-3.1-8b-instruct.
  name: model
  type: string
- description: ''
  name: messages
  type: array
- description: Maximum number of tokens to generate.
  name: max_tokens
  type: integer
- description: Sampling temperature between 0 and 2.
  name: temperature
  type: number
- description: Nucleus sampling parameter.
  name: top_p
  type: number
- description: Whether to stream the response via server-sent events.
  name: stream
  type: boolean
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-workers-ai-chat-completion-request-schema.json
slug: cloudflare-workers-ai-chat-completion-request
source_filename: cloudflare-workers-ai-chat-completion-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model identifier, e.g. @cf/meta/llama-3.1-8b-instruct.\"\n    },\n    \"messages\": {\n      \"type\": \"array\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of tokens to generate.\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Sampling temperature between 0 and 2.\"\n    },\n    \"top_p\": {\n      \"type\": \"number\",\n      \"description\": \"Nucleus sampling parameter.\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to stream the response via server-sent events.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-workers-ai-chat-completion-request-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: ChatCompletionRequest
---
