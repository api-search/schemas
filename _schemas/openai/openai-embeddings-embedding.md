---
description: ''
layout: schema
name: Embedding
properties_list:
- description: The object type, always embedding.
  name: object
  type: string
- description: ''
  name: embedding
  type: string
- description: The index of the embedding in the list of embeddings, corresponding to the position of the input.
  name: index
  type: integer
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-embeddings-embedding-schema.json
slug: openai-embeddings-embedding
source_filename: openai-embeddings-embedding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Embedding\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The object type, always embedding.\"\n    },\n    \"embedding\": {\n      \"type\": \"string\"\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the embedding in the list of embeddings, corresponding to the position of the input.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-embeddings-embedding-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: Embedding
---
