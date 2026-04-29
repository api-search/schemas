---
description: ''
layout: schema
name: ModelSummary
properties_list:
- description: Unique model identifier
  name: _id
  type: string
- description: Model repository ID (e.g., bert-base-uncased)
  name: id
  type: string
- description: Alias for id
  name: modelId
  type: string
- description: Model author or organization
  name: author
  type: string
- description: Latest commit SHA
  name: sha
  type: string
- description: Last modification timestamp
  name: lastModified
  type: string
- description: Whether the model is private
  name: private
  type: boolean
- description: ''
  name: disabled
  type: boolean
- description: Whether access is gated
  name: gated
  type: boolean
- description: Pipeline task tag
  name: pipeline_tag
  type: string
- description: ''
  name: tags
  type: array
- description: Total download count
  name: downloads
  type: integer
- description: Total like count
  name: likes
  type: integer
- description: Primary ML library
  name: library_name
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-hub-model-summary-schema.json
slug: hugging-face-hub-model-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModelSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique model identifier\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Model repository ID (e.g., bert-base-uncased)\"\n    },\n    \"modelId\": {\n      \"type\": \"string\",\n      \"description\": \"Alias for id\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Model author or organization\"\n    },\n    \"sha\": {\n      \"type\": \"string\",\n      \"description\": \"Latest commit SHA\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"description\": \"Last modification timestamp\"\n    },\n    \"private\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the model is private\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"gated\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether access is gated\"\n    },\n    \"pipeline_tag\": {\n      \"type\": \"string\",\n      \"description\": \"Pipeline task tag\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"downloads\": {\n      \"type\": \"integer\",\n      \"description\": \"Total download count\"\n    },\n    \"likes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total like count\"\n    },\n    \"library_name\": {\n      \"type\": \"string\",\n      \"description\": \"Primary ML library\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-hub-model-summary-schema.json
tags: []
title: ModelSummary
---
