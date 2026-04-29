---
description: A single message in a chat conversation.
layout: schema
name: ChatMessage
properties_list:
- description: Role of the message author.
  name: role
  type: string
- description: Content of the message.
  name: content
  type: string
provider_name: Bifrost
provider_slug: bifrost
schema_file: json-schema/bifrost-chat-message-schema.json
slug: bifrost-chat-message
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ChatMessage\",\n  \"type\": \"object\",\n  \"description\": \"A single message in a chat conversation.\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role of the message author.\",\n      \"enum\": [\n        \"system\",\n        \"user\",\n        \"assistant\"\n      ],\n      \"example\": \"user\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Content of the message.\",\n      \"example\": \"Hello, how are you?\"\n    }\n  },\n  \"required\": [\n    \"role\",\n    \"content\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/json-schema/bifrost-chat-message-schema.json
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
title: ChatMessage
---
