---
description: ''
layout: schema
name: EmbeddingResponse
properties_list:
- description: ''
  name: object
  type: string
- description: ''
  name: data
  type: array
- description: ''
  name: model
  type: string
- description: ''
  name: usage
  type: object
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-providers-embedding-response-schema.json
slug: hugging-face-inference-providers-embedding-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmbeddingResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\"\n    },\n    \"data\": {\n      \"type\": \"array\"\n    },\n    \"model\": {\n      \"type\": \"string\"\n    },\n    \"usage\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-providers-embedding-response-schema.json
tags: []
title: EmbeddingResponse
---
