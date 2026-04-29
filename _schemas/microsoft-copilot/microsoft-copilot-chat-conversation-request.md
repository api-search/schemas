---
description: ''
layout: schema
name: ChatConversationRequest
properties_list:
- description: Natural language prompt to send to Microsoft 365 Copilot to start a conversation.
  name: prompt
  type: string
- description: Whether to enable web search grounding for this message. Defaults to true. Must be toggled off per message if not desired.
  name: enableWebSearch
  type: boolean
- description: Optional OneDrive and SharePoint file references to provide as additional context.
  name: fileReferences
  type: array
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-chat-conversation-request-schema.json
slug: microsoft-copilot-chat-conversation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChatConversationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Natural language prompt to send to Microsoft 365 Copilot to start a conversation.\"\n    },\n    \"enableWebSearch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable web search grounding for this message. Defaults to true. Must be toggled off per message if not desired.\"\n    },\n    \"fileReferences\": {\n      \"type\": \"array\",\n      \"description\": \"Optional OneDrive and SharePoint file references to provide as additional context.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-chat-conversation-request-schema.json
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
title: ChatConversationRequest
---
