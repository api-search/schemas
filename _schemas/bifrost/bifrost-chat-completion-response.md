---
description: Response from a chat completion request.
layout: schema
name: ChatCompletionResponse
properties_list:
- description: Unique identifier for the completion.
  name: id
  type: string
- description: Object type, always chat.completion.
  name: object
  type: string
- description: Unix timestamp of when the completion was created.
  name: created
  type: integer
- description: Provider and model used for the completion.
  name: model
  type: string
- description: Array of completion choices.
  name: choices
  type: array
- description: ''
  name: usage
  type: object
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-chat-completion-response-schema.json
slug: bifrost-chat-completion-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ChatCompletionResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from a chat completion request.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the completion.\",\n      \"example\": \"chatcmpl-abc123\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"Object type, always chat.completion.\",\n      \"example\": \"chat.completion\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the completion was created.\",\n      \"example\": 1713000000\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Provider and model used for the completion.\",\n      \"example\": \"openai/gpt-4o\"\n    },\n    \"choices\": {\n      \"type\": \"array\",\n      \"description\": \"Array of completion choices.\",\n      \"\
  items\": {\n        \"$ref\": \"#/components/schemas/ChatChoice\"\n      }\n    },\n    \"usage\": {\n      \"$ref\": \"#/components/schemas/UsageStats\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/json-schema/bifrost-chat-completion-response-schema.json
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: ChatCompletionResponse
---
