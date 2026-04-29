---
description: ''
layout: schema
name: Chat Conversation
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: participantIds
  type: array
provider_name: Chat
provider_slug: chat
schema_file: json-schema/chat-conversation-schema.json
slug: chat-conversation
source_filename: chat-conversation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://apievangelist.com/schemas/chat/conversation.json\",\n  \"title\": \"Chat Conversation\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"title\": { \"type\": \"string\" },\n    \"createdAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"updatedAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"participantIds\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chat/refs/heads/main/json-schema/chat-conversation-schema.json
tags:
- Chat
- Conversational AI
- Conversations
- Customer Support
- Messaging
- Real-time
title: Chat Conversation
---
