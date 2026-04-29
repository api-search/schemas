---
description: Request body for creating text embeddings via AIMLAPI
layout: schema
name: EmbeddingRequest
properties_list:
- description: Embedding model ID
  name: model
  type: string
- description: Text to embed
  name: input
  type: string
- description: Encoding format (float, base64)
  name: encoding_format
  type: string
- description: Output embedding dimensions
  name: dimensions
  type: integer
provider_name: AIMLAPI
provider_slug: aimlapi
schema_file: json-schema/aimlapi-embedding-request-schema.json
slug: aimlapi-embedding-request
source_filename: aimlapi-embedding-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-embedding-request-schema.json\",\n  \"title\": \"EmbeddingRequest\",\n  \"description\": \"Request body for creating text embeddings via AIMLAPI\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Embedding model ID\",\n      \"example\": \"text-embedding-3-small\"\n    },\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"Text to embed\",\n      \"example\": \"The quick brown fox jumps over the lazy dog\"\n    },\n    \"encoding_format\": {\n      \"type\": \"string\",\n      \"description\": \"Encoding format (float, base64)\",\n      \"example\": \"float\"\n    },\n    \"dimensions\": {\n      \"type\": \"integer\",\n      \"description\": \"Output embedding dimensions\",\n      \"example\": 1536\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/json-schema/aimlapi-embedding-request-schema.json
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
title: EmbeddingRequest
---
