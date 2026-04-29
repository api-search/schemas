---
description: Information about an available AI model
layout: schema
name: ModelInfo
properties_list:
- description: Model identifier
  name: id
  type: string
- description: Object type
  name: object
  type: string
- description: Unix timestamp of model creation
  name: created
  type: integer
- description: Organization that owns/created the model
  name: owned_by
  type: string
provider_name: AIMLAPI
provider_slug: aimlapi
schema_file: json-schema/aimlapi-model-info-schema.json
slug: aimlapi-model-info
source_filename: aimlapi-model-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-model-info-schema.json\",\n  \"title\": \"ModelInfo\",\n  \"description\": \"Information about an available AI model\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Model identifier\",\n      \"example\": \"gpt-4o\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"Object type\",\n      \"example\": \"model\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of model creation\",\n      \"example\": 1718153645\n    },\n    \"owned_by\": {\n      \"type\": \"string\",\n      \"description\": \"Organization that owns/created the model\",\n      \"example\": \"openai\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-model-info-schema.json
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
title: ModelInfo
---
