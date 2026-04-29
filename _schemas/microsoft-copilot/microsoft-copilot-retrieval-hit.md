---
description: ''
layout: schema
name: RetrievalHit
properties_list:
- description: The URL of the source document.
  name: webUrl
  type: string
- description: Collection of relevant text extracts from the document.
  name: extracts
  type: array
- description: The type of resource. Values include listItem (for SharePoint/OneDrive) and externalItem (for Copilot connectors).
  name: resourceType
  type: string
- description: Metadata fields for the resource, as requested via the resourceMetadata parameter. Keys and values depend on the requested fields.
  name: resourceMetadata
  type: object
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-retrieval-hit-schema.json
slug: microsoft-copilot-retrieval-hit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RetrievalHit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the source document.\"\n    },\n    \"extracts\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of relevant text extracts from the document.\"\n    },\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of resource. Values include listItem (for SharePoint/OneDrive) and externalItem (for Copilot connectors).\"\n    },\n    \"resourceMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata fields for the resource, as requested via the resourceMetadata parameter. Keys and values depend on the requested fields.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-retrieval-hit-schema.json
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
title: RetrievalHit
---
