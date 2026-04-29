---
description: ''
layout: schema
name: RetrievalExtract
properties_list:
- description: The relevant text extract from the document.
  name: text
  type: string
- description: Cosine similarity between the queryString and the extract, normalized to the 0-1 range. May be absent for Copilot connectors results.
  name: relevanceScore
  type: number
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-retrieval-extract-schema.json
slug: microsoft-copilot-retrieval-extract
source_filename: microsoft-copilot-retrieval-extract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RetrievalExtract\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The relevant text extract from the document.\"\n    },\n    \"relevanceScore\": {\n      \"type\": \"number\",\n      \"description\": \"Cosine similarity between the queryString and the extract, normalized to the 0-1 range. May be absent for Copilot connectors results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-retrieval-extract-schema.json
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
title: RetrievalExtract
---
