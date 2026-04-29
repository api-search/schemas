---
description: ''
layout: schema
name: ChatMessage
properties_list:
- description: The unique identifier for the message.
  name: id
  type: string
- description: ''
  name: body
  type: object
- description: Sources referenced in the Copilot response.
  name: citations
  type: array
- description: The timestamp when the message was created.
  name: createdDateTime
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-chat-message-schema.json
slug: microsoft-copilot-chat-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatMessage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the message.\"\n    },\n    \"body\": {\n      \"type\": \"object\"\n    },\n    \"citations\": {\n      \"type\": \"array\",\n      \"description\": \"Sources referenced in the Copilot response.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the message was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-chat-message-schema.json
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft 365
- Productivity
title: ChatMessage
---
