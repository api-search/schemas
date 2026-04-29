---
description: ''
layout: schema
name: SearchResponse
properties_list:
- description: URL to retrieve the next page of results, if available.
  name: '@odata.nextLink'
  type: string
- description: Total number of matching results.
  name: totalCount
  type: integer
- description: Collection of search result items.
  name: searchHits
  type: array
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-search-response-schema.json
slug: microsoft-copilot-search-response
source_filename: microsoft-copilot-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"URL to retrieve the next page of results, if available.\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching results.\"\n    },\n    \"searchHits\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of search result items.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-search-response-schema.json
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
title: SearchResponse
---
