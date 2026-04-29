---
description: ''
layout: schema
name: Chat Message
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: conversationId
  type: string
- description: ''
  name: senderId
  type: string
- description: ''
  name: content
  type: string
- description: ''
  name: contentType
  type: string
- description: ''
  name: sentAt
  type: string
- description: ''
  name: editedAt
  type: string
- description: ''
  name: metadata
  type: object
provider_name: Chat
provider_slug: chat
schema_file: json-schema/chat-message-schema.json
slug: chat-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://apievangelist.com/schemas/chat/message.json\",\n  \"title\": \"Chat Message\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"content\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"conversationId\": { \"type\": \"string\" },\n    \"senderId\": { \"type\": \"string\" },\n    \"content\": { \"type\": \"string\" },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"enum\": [\"text\", \"markdown\", \"html\"]\n    },\n    \"sentAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"editedAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"metadata\": { \"type\": \"object\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chat/refs/heads/main/json-schema/chat-message-schema.json
tags:
- Chat
- Conversational AI
- Conversations
- Customer Support
- Messaging
- Real-time
title: Chat Message
---
