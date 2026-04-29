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
- description: The Unix timestamp (in seconds) of when the completion was created.
  name: created
  type: integer
- description: The model used for the chat completion.
  name: model
  type: string
- description: A list of chat completion choices.
  name: choices
  type: array
- description: This fingerprint represents the backend configuration that the model runs with. Can be used with the seed parameter to detect backend changes.
  name: system_fingerprint
  type: string
- description: The service tier used for processing the request.
  name: service_tier
  type: string
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-chat-completions-create-chat-completion-response-schema.json
slug: openai-chat-completions-create-chat-completion-response
source_filename: openai-chat-completions-create-chat-completion-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateChatCompletionResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the chat completion.\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type, always chat.completion.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"The Unix timestamp (in seconds) of when the completion was created.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model used for the chat completion.\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"description\": \"A list of chat completion choices.\"\n    },\n    \"system_fingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"This fingerprint represents the backend configuration that the model runs with. Can be used with\
  \ the seed parameter to detect backend changes.\"\n    },\n    \"service_tier\": {\n      \"type\": \"string\",\n      \"description\": \"The service tier used for processing the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-chat-completions-create-chat-completion-response-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: CreateChatCompletionResponse
---
