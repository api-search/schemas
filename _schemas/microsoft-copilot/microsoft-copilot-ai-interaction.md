---
description: Represents an interaction between a user and Copilot across Microsoft 365 applications.
layout: schema
name: AiInteraction
properties_list:
- description: The unique identifier for the interaction message.
  name: id
  type: string
- description: The data source for Copilot data. For example, IPM.SkypeTeams.Message.Copilot.Excel or IPM.SkypeTeams.Message.Copilot.Loop.
  name: appClass
  type: string
- description: Indicates whether the interaction is a user prompt or a Copilot response.
  name: interactionType
  type: string
- description: The type of the conversation (e.g., appchat, bizchat).
  name: conversationType
  type: string
- description: Identifier that groups a user prompt with its corresponding Copilot response.
  name: requestId
  type: string
- description: Thread ID or conversation identifier that maps to all Copilot sessions for the user.
  name: sessionId
  type: string
- description: The time when the interaction was created.
  name: createdDateTime
  type: string
- description: Timestamp of when the interaction was last modified.
  name: etag
  type: string
- description: The locale of the sender.
  name: locale
  type: string
- description: Collection of documents attached to the interaction, such as cards and images.
  name: attachments
  type: array
- description: Identifiers that map to all contexts associated with the interaction.
  name: contexts
  type: array
- description: Collection of links that appear in the interaction.
  name: links
  type: array
- description: Collection of entities mentioned in the interaction, including users and bots.
  name: mentions
  type: array
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-ai-interaction-schema.json
slug: microsoft-copilot-ai-interaction
source_filename: microsoft-copilot-ai-interaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AiInteraction\",\n  \"type\": \"object\",\n  \"description\": \"Represents an interaction between a user and Copilot across Microsoft 365 applications.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the interaction message.\"\n    },\n    \"appClass\": {\n      \"type\": \"string\",\n      \"description\": \"The data source for Copilot data. For example, IPM.SkypeTeams.Message.Copilot.Excel or IPM.SkypeTeams.Message.Copilot.Loop.\"\n    },\n    \"interactionType\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the interaction is a user prompt or a Copilot response.\"\n    },\n    \"conversationType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the conversation (e.g., appchat, bizchat).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Identifier that groups a user prompt with its corresponding Copilot response.\"\n    },\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Thread ID or conversation identifier that maps to all Copilot sessions for the user.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time when the interaction was created.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the interaction was last modified.\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"The locale of the sender.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of documents attached to the interaction, such as cards and images.\"\n    },\n    \"contexts\": {\n      \"type\": \"array\",\n      \"description\": \"Identifiers that map to all contexts associated with the interaction.\"\n    },\n    \"links\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"Collection of links that appear in the interaction.\"\n    },\n    \"mentions\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of entities mentioned in the interaction, including users and bots.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-ai-interaction-schema.json
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
title: AiInteraction
---
