---
description: ''
layout: schema
name: EmbeddingRequest
properties_list:
- description: Embedding model ID
  name: model
  type: string
- description: Text input(s) to embed
  name: input
  type: string
- description: ''
  name: encoding_format
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-providers-embedding-request-schema.json
slug: hugging-face-inference-providers-embedding-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmbeddingRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Embedding model ID\"\n    },\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"Text input(s) to embed\"\n    },\n    \"encoding_format\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-providers-embedding-request-schema.json
tags: []
title: EmbeddingRequest
---
