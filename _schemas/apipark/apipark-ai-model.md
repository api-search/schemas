---
description: Schema representing an AI model integrated with the APIPark AI gateway
layout: schema
name: APIPark AI Model
properties_list:
- description: Unique identifier of the AI model integration
  name: id
  type: string
- description: AI provider name (e.g., OpenAI, Anthropic, Gemini)
  name: provider
  type: string
- description: Name of the AI model
  name: modelName
  type: string
- description: ''
  name: status
  type: string
- description: Load balancing priority
  name: priority
  type: integer
provider_name: APIPark
provider_slug: apipark
schema_file: json-schema/apipark-ai-model-schema.json
slug: apipark-ai-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apipark/main/json-schema/apipark-ai-model-schema.json\",\n  \"title\": \"APIPark AI Model\",\n  \"description\": \"Schema representing an AI model integrated with the APIPark AI gateway\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier of the AI model integration\" },\n    \"provider\": { \"type\": \"string\", \"description\": \"AI provider name (e.g., OpenAI, Anthropic, Gemini)\" },\n    \"modelName\": { \"type\": \"string\", \"description\": \"Name of the AI model\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"active\", \"inactive\"] },\n    \"priority\": { \"type\": \"integer\", \"description\": \"Load balancing priority\" }\n  },\n  \"required\": [\"id\", \"provider\", \"modelName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/json-schema/apipark-ai-model-schema.json
tags:
- AI Gateway
- API Gateway
- API Management
- Developer Portal
- LLM
- Open Source
title: APIPark AI Model
---
