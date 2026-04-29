---
description: ''
layout: schema
name: CompletionUsage
properties_list:
- description: Number of tokens in the prompt.
  name: prompt_tokens
  type: integer
- description: Number of tokens in the generated completion.
  name: completion_tokens
  type: integer
- description: Total number of tokens used in the request.
  name: total_tokens
  type: integer
- description: Breakdown of tokens used in a completion.
  name: completion_tokens_details
  type: object
- description: Breakdown of tokens used in the prompt.
  name: prompt_tokens_details
  type: object
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-completion-usage-schema.json
slug: chatgpt-chat-completions-completion-usage
source_filename: chatgpt-chat-completions-completion-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompletionUsage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the prompt.\"\n    },\n    \"completion_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tokens in the generated completion.\"\n    },\n    \"total_tokens\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of tokens used in the request.\"\n    },\n    \"completion_tokens_details\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of tokens used in a completion.\"\n    },\n    \"prompt_tokens_details\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of tokens used in the prompt.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-completion-usage-schema.json
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
title: CompletionUsage
---
