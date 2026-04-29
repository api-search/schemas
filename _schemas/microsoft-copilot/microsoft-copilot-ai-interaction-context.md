---
description: Represents context associated with an interaction.
layout: schema
name: AiInteractionContext
properties_list:
- description: The full file URL where the interaction happened.
  name: contextReference
  type: string
- description: The type of the file.
  name: contextType
  type: string
- description: The name of the file.
  name: displayName
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-ai-interaction-context-schema.json
slug: microsoft-copilot-ai-interaction-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AiInteractionContext\",\n  \"type\": \"object\",\n  \"description\": \"Represents context associated with an interaction.\",\n  \"properties\": {\n    \"contextReference\": {\n      \"type\": \"string\",\n      \"description\": \"The full file URL where the interaction happened.\"\n    },\n    \"contextType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the file.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-ai-interaction-context-schema.json
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
title: AiInteractionContext
---
