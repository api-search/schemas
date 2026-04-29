---
description: An AIMLAPI API key for authentication
layout: schema
name: ApiKey
properties_list:
- description: API key identifier
  name: id
  type: string
- description: Human-readable key name
  name: name
  type: string
- description: The API key value (only shown on creation)
  name: key
  type: string
- description: Creation timestamp
  name: created_at
  type: string
- description: 'Key status: active, disabled'
  name: status
  type: string
provider_name: AIMLAPI
provider_slug: aimlapi
schema_file: json-schema/aimlapi-api-key-schema.json
slug: aimlapi-api-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-api-key-schema.json\",\n  \"title\": \"ApiKey\",\n  \"description\": \"An AIMLAPI API key for authentication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"API key identifier\",\n      \"example\": \"key-abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable key name\",\n      \"example\": \"Production Key\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The API key value (only shown on creation)\",\n      \"example\": \"aiml-sk-examplekey123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"status\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Key status: active, disabled\",\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-api-key-schema.json
tags:
- Artificial Intelligence
- Machine Learning
- AI Models
- LLM
- Image Generation
- Video Generation
- Speech
- Embeddings
- API Gateway
- Developer Tools
title: ApiKey
---
