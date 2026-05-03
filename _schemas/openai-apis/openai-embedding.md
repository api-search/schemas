---
description: Represents an embedding vector returned by the embedding endpoint, containing the numerical vector representation and its index.
layout: schema
name: OpenAI Embedding
properties_list:
- description: The object type, always embedding
  name: object
  type: string
- description: The embedding vector representing the input text
  name: embedding
  type: object
- description: The index of the embedding in the list of embeddings
  name: index
  type: integer
provider_name: OpenAI APIs
provider_slug: openai-apis
schema_file: json-schema/openai-embedding-schema.json
slug: openai-embedding
source_filename: openai-embedding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.openai.com/schemas/openai/embedding.json\",\n  \"title\": \"OpenAI Embedding\",\n  \"description\": \"Represents an embedding vector returned by the embedding endpoint, containing the numerical vector representation and its index.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"embedding\",\n      \"description\": \"The object type, always embedding\"\n    },\n    \"embedding\": {\n      \"oneOf\": [\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"number\"\n          },\n          \"description\": \"The embedding vector as an array of floats\"\n        },\n        {\n          \"type\": \"string\",\n          \"description\": \"The embedding vector as a base64-encoded string\"\n        }\n      ],\n      \"description\": \"The embedding vector representing the input text\"\
  \n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the embedding in the list of embeddings\"\n    }\n  },\n  \"required\": [\"object\", \"embedding\", \"index\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/json-schema/openai-embedding-schema.json
tags:
- Artificial Intelligence
- Embeddings
- Image Generation
- Language Models
- Speech
title: OpenAI Embedding
---
