---
description: ''
layout: schema
name: SearchHit
properties_list:
- description: The URL of the matching document.
  name: webUrl
  type: string
- description: A preview snippet of the matching content.
  name: preview
  type: string
- description: The type of resource (e.g., driveItem).
  name: resourceType
  type: string
- description: Metadata fields for the resource, if requested.
  name: resourceMetadata
  type: object
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-search-hit-schema.json
slug: microsoft-copilot-search-hit
source_filename: microsoft-copilot-search-hit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchHit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the matching document.\"\n    },\n    \"preview\": {\n      \"type\": \"string\",\n      \"description\": \"A preview snippet of the matching content.\"\n    },\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of resource (e.g., driveItem).\"\n    },\n    \"resourceMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata fields for the resource, if requested.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-search-hit-schema.json
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
title: SearchHit
---
