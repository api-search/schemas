---
description: Represents a link that appears in an AI interaction.
layout: schema
name: AiInteractionLink
properties_list:
- description: The name of the link.
  name: displayName
  type: string
- description: Information about a link in an app chat or Business Chat (BizChat) interaction.
  name: linkType
  type: string
- description: The URL of the link.
  name: linkUrl
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-ai-interaction-link-schema.json
slug: microsoft-copilot-ai-interaction-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AiInteractionLink\",\n  \"type\": \"object\",\n  \"description\": \"Represents a link that appears in an AI interaction.\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the link.\"\n    },\n    \"linkType\": {\n      \"type\": \"string\",\n      \"description\": \"Information about a link in an app chat or Business Chat (BizChat) interaction.\"\n    },\n    \"linkUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the link.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-ai-interaction-link-schema.json
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
title: AiInteractionLink
---
