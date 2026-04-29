---
description: ''
layout: schema
name: ChatCompletionToolCall
properties_list:
- description: The ID of the tool call.
  name: id
  type: string
- description: The type of the tool call.
  name: type
  type: string
- description: ''
  name: function
  type: object
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-chat-completion-tool-call-schema.json
slug: chatgpt-chat-completions-chat-completion-tool-call
source_filename: chatgpt-chat-completions-chat-completion-tool-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatCompletionToolCall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the tool call.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the tool call.\"\n    },\n    \"function\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-chat-completion-tool-call-schema.json
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
title: ChatCompletionToolCall
---
