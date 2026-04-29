---
description: ''
layout: schema
name: CreateChatCompletionResponse
properties_list:
- description: A unique identifier for the chat completion.
  name: id
  type: string
- description: The object type, always chat.completion.
  name: object
  type: string
- description: The Unix timestamp (in seconds) of when the chat completion was created.
  name: created
  type: integer
- description: The model used for the chat completion.
  name: model
  type: string
- description: A list of chat completion choices. Can be more than one if n is greater than 1.
  name: choices
  type: array
- description: This fingerprint represents the backend configuration that the model runs with. Can be used with the seed parameter to understand when backend changes have been made.
  name: system_fingerprint
  type: string
- description: The service tier used for processing the request.
  name: service_tier
  type: string
provider_name: ChatGPT
provider_slug: chatgpt
schema_file: json-schema/chatgpt-chat-completions-create-chat-completion-response-schema.json
slug: chatgpt-chat-completions-create-chat-completion-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateChatCompletionResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the chat completion.\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type, always chat.completion.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp (in seconds) of when the chat completion\\nwas created.\\n\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model used for the chat completion.\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"description\": \"A list of chat completion choices. Can be more than one\\nif n is greater than 1.\\n\"\n    },\n    \"system_fingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"This fingerprint represents the backend\
  \ configuration that\\nthe model runs with. Can be used with the seed parameter\\nto understand when backend changes have been made.\\n\"\n    },\n    \"service_tier\": {\n      \"type\": \"string\",\n      \"description\": \"The service tier used for processing the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/json-schema/chatgpt-chat-completions-create-chat-completion-response-schema.json
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
title: CreateChatCompletionResponse
---
