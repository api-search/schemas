---
description: The body of a message.
layout: schema
name: ItemBody
properties_list:
- description: The type of the content.
  name: contentType
  type: string
- description: The content of the body.
  name: content
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-item-body-schema.json
slug: microsoft-copilot-item-body
source_filename: microsoft-copilot-item-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ItemBody\",\n  \"type\": \"object\",\n  \"description\": \"The body of a message.\",\n  \"properties\": {\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the content.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the body.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-item-body-schema.json
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
title: ItemBody
---
