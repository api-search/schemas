---
description: ''
layout: schema
name: ResponseOutputContentPart
properties_list:
- description: The type of the content part.
  name: type
  type: string
- description: The text content.
  name: text
  type: string
- description: The refusal text.
  name: refusal
  type: string
- description: Annotations on the text, such as citations from file search or web search.
  name: annotations
  type: array
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-response-output-content-part-schema.json
slug: chatgpt-responses-response-output-content-part
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseOutputContentPart\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the content part.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content.\"\n    },\n    \"refusal\": {\n      \"type\": \"string\",\n      \"description\": \"The refusal text.\"\n    },\n    \"annotations\": {\n      \"type\": \"array\",\n      \"description\": \"Annotations on the text, such as citations from file\\nsearch or web search.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-response-output-content-part-schema.json
tags:
- Agents
- AI
- ChatGPT
- Embeddings
- Fine-Tuning
- GPT-4
- GPT-5
- Language Model
- OpenAI
- Realtime
title: ResponseOutputContentPart
---
