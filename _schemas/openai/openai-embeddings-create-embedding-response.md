---
description: ''
layout: schema
name: CreateEmbeddingResponse
properties_list:
- description: The object type, always list.
  name: object
  type: string
- description: The list of embedding objects.
  name: data
  type: array
- description: The name of the model used to generate the embedding.
  name: model
  type: string
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-embeddings-create-embedding-response-schema.json
slug: openai-embeddings-create-embedding-response
source_filename: openai-embeddings-create-embedding-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateEmbeddingResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type, always list.\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of embedding objects.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the model used to generate the embedding.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-embeddings-create-embedding-response-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: CreateEmbeddingResponse
---
