---
description: ''
layout: schema
name: SearchRequest
properties_list:
- description: Natural language query to search for relevant files.
  name: query
  type: string
- description: Number of results to return per page (1-100). Default is 25.
  name: pageSize
  type: integer
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-search-request-schema.json
slug: microsoft-copilot-search-request
source_filename: microsoft-copilot-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Natural language query to search for relevant files.\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results to return per page (1-100). Default is 25.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-search-request-schema.json
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
title: SearchRequest
---
