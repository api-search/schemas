---
description: Represents a message attachment such as cards and images.
layout: schema
name: AiInteractionAttachment
properties_list:
- description: Identifier for the attachment, unique only within the message scope.
  name: attachmentId
  type: string
- description: The content of the attachment.
  name: content
  type: string
- description: The type of the content (e.g., reference, file, image/imageType).
  name: contentType
  type: string
- description: The URL of the content.
  name: contentUrl
  type: string
- description: The name of the attachment.
  name: name
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-ai-interaction-attachment-schema.json
slug: microsoft-copilot-ai-interaction-attachment
source_filename: microsoft-copilot-ai-interaction-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AiInteractionAttachment\",\n  \"type\": \"object\",\n  \"description\": \"Represents a message attachment such as cards and images.\",\n  \"properties\": {\n    \"attachmentId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the attachment, unique only within the message scope.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the attachment.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the content (e.g., reference, file, image/imageType).\"\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the content.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the attachment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-ai-interaction-attachment-schema.json
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
title: AiInteractionAttachment
---
