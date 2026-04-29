---
description: ''
layout: schema
name: ResponseToolChoice
properties_list:
- description: The type of tool to force.
  name: type
  type: string
- description: The name of the function to call. Required when type is function.
  name: name
  type: string
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-responses-response-tool-choice-schema.json
slug: chatgpt-responses-response-tool-choice
source_filename: chatgpt-responses-response-tool-choice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseToolChoice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of tool to force.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the function to call. Required when type\\nis function.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-responses-response-tool-choice-schema.json
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
title: ResponseToolChoice
---
