---
description: An object specifying the format that the model must output. Setting to json_schema enables Structured Outputs which ensures the model will match your supplied JSON schema.
layout: schema
name: ResponseFormat
properties_list:
- description: The type of response format.
  name: type
  type: string
- description: The JSON schema the model must conform to. Required when type is json_schema.
  name: json_schema
  type: object
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-response-format-schema.json
slug: chatgpt-chat-completions-response-format
source_filename: chatgpt-chat-completions-response-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseFormat\",\n  \"type\": \"object\",\n  \"description\": \"An object specifying the format that the model must output.\\nSetting to json_schema enables Structured Outputs which ensures\\nthe model will match your supplied JSON schema.\\n\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of response format.\"\n    },\n    \"json_schema\": {\n      \"type\": \"object\",\n      \"description\": \"The JSON schema the model must conform to. Required when\\ntype is json_schema.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-response-format-schema.json
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
title: ResponseFormat
---
