---
description: ''
layout: schema
name: ChatCompletionResponse
properties_list:
- description: Unique identifier for the completion.
  name: id
  type: string
- description: ''
  name: object
  type: string
- description: Unix timestamp of when the completion was created.
  name: created
  type: integer
- description: The model used for the completion.
  name: model
  type: string
- description: ''
  name: choices
  type: array
- description: ''
  name: usage
  type: object
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-workers-ai-chat-completion-response-schema.json
slug: cloudflare-workers-ai-chat-completion-response
source_filename: cloudflare-workers-ai-chat-completion-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the completion.\"\n    },\n    \"object\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the completion was created.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model used for the completion.\"\n    },\n    \"choices\": {\n      \"type\": \"array\"\n    },\n    \"usage\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-workers-ai-chat-completion-response-schema.json
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
title: ChatCompletionResponse
---
