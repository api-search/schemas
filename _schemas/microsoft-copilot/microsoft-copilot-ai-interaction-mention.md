---
description: Represents a mention of an entity in an AI interaction.
layout: schema
name: AiInteractionMention
properties_list:
- description: The entity mentioned in the message.
  name: mentioned
  type: object
- description: The identifier for the mention.
  name: mentionId
  type: integer
- description: The text mentioned in the message.
  name: mentionText
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-ai-interaction-mention-schema.json
slug: microsoft-copilot-ai-interaction-mention
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AiInteractionMention\",\n  \"type\": \"object\",\n  \"description\": \"Represents a mention of an entity in an AI interaction.\",\n  \"properties\": {\n    \"mentioned\": {\n      \"type\": \"object\",\n      \"description\": \"The entity mentioned in the message.\"\n    },\n    \"mentionId\": {\n      \"type\": \"integer\",\n      \"description\": \"The identifier for the mention.\"\n    },\n    \"mentionText\": {\n      \"type\": \"string\",\n      \"description\": \"The text mentioned in the message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-ai-interaction-mention-schema.json
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
title: AiInteractionMention
---
