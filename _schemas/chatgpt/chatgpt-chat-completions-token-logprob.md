---
description: ''
layout: schema
name: TokenLogprob
properties_list:
- description: The token.
  name: token
  type: string
- description: The log probability of this token.
  name: logprob
  type: number
- description: A list of integers representing the UTF-8 bytes representation of the token.
  name: bytes
  type: array
- description: List of the most likely tokens and their log probability.
  name: top_logprobs
  type: array
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-token-logprob-schema.json
slug: chatgpt-chat-completions-token-logprob
source_filename: chatgpt-chat-completions-token-logprob-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TokenLogprob\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The token.\"\n    },\n    \"logprob\": {\n      \"type\": \"number\",\n      \"description\": \"The log probability of this token.\"\n    },\n    \"bytes\": {\n      \"type\": \"array\",\n      \"description\": \"A list of integers representing the UTF-8 bytes\\nrepresentation of the token.\\n\"\n    },\n    \"top_logprobs\": {\n      \"type\": \"array\",\n      \"description\": \"List of the most likely tokens and their log probability.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-token-logprob-schema.json
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
title: TokenLogprob
---
