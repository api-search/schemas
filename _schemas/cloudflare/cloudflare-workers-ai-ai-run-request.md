---
description: ''
layout: schema
name: AiRunRequest
properties_list:
- description: The input prompt for text generation models.
  name: prompt
  type: string
- description: Array of messages for chat-style models.
  name: messages
  type: array
- description: Raw image bytes for image classification models.
  name: image
  type: array
- description: Text input for embedding or translation models.
  name: text
  type: string
- description: Source language code for translation.
  name: source_lang
  type: string
- description: Target language code for translation.
  name: target_lang
  type: string
- description: Maximum number of tokens to generate.
  name: max_tokens
  type: integer
- description: Sampling temperature.
  name: temperature
  type: number
- description: Whether to stream the response using server-sent events.
  name: stream
  type: boolean
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-workers-ai-ai-run-request-schema.json
slug: cloudflare-workers-ai-ai-run-request
source_filename: cloudflare-workers-ai-ai-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AiRunRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"The input prompt for text generation models.\"\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"description\": \"Array of messages for chat-style models.\"\n    },\n    \"image\": {\n      \"type\": \"array\",\n      \"description\": \"Raw image bytes for image classification models.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Text input for embedding or translation models.\"\n    },\n    \"source_lang\": {\n      \"type\": \"string\",\n      \"description\": \"Source language code for translation.\"\n    },\n    \"target_lang\": {\n      \"type\": \"string\",\n      \"description\": \"Target language code for translation.\"\n    },\n    \"max_tokens\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Maximum number of tokens to generate.\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"Sampling temperature.\"\n    },\n    \"stream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to stream the response using server-sent events.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-workers-ai-ai-run-request-schema.json
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
title: AiRunRequest
---
