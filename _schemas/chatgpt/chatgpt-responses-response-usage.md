---
description: ''
layout: schema
name: ResponseUsage
properties_list:
- description: The number of input tokens used.
  name: input_tokens
  type: integer
- description: A detailed breakdown of input token usage.
  name: input_tokens_details
  type: object
- description: The number of output tokens generated.
  name: output_tokens
  type: integer
- description: A detailed breakdown of output token usage.
  name: output_tokens_details
  type: object
- description: The total number of tokens used.
  name: total_tokens
  type: integer
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-response-usage-schema.json
slug: chatgpt-responses-response-usage
source_filename: chatgpt-responses-response-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseUsage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"input_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of input tokens used.\"\n    },\n    \"input_tokens_details\": {\n      \"type\": \"object\",\n      \"description\": \"A detailed breakdown of input token usage.\"\n    },\n    \"output_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of output tokens generated.\"\n    },\n    \"output_tokens_details\": {\n      \"type\": \"object\",\n      \"description\": \"A detailed breakdown of output token usage.\"\n    },\n    \"total_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of tokens used.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-response-usage-schema.json
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
title: ResponseUsage
---
