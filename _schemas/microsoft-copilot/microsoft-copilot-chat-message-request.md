---
description: ''
layout: schema
name: ChatMessageRequest
properties_list:
- description: Natural language prompt to continue the conversation.
  name: prompt
  type: string
- description: Whether to enable web search grounding for this message.
  name: enableWebSearch
  type: boolean
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-chat-message-request-schema.json
slug: microsoft-copilot-chat-message-request
source_filename: microsoft-copilot-chat-message-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatMessageRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Natural language prompt to continue the conversation.\"\n    },\n    \"enableWebSearch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable web search grounding for this message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-chat-message-request-schema.json
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
title: ChatMessageRequest
---
