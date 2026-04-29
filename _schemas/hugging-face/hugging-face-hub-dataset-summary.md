---
description: ''
layout: schema
name: DatasetSummary
properties_list:
- description: ''
  name: _id
  type: string
- description: Dataset repository ID
  name: id
  type: string
- description: ''
  name: author
  type: string
- description: ''
  name: sha
  type: string
- description: ''
  name: lastModified
  type: string
- description: ''
  name: private
  type: boolean
- description: ''
  name: gated
  type: boolean
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: tags
  type: array
- description: ''
  name: downloads
  type: integer
- description: ''
  name: likes
  type: integer
- description: ''
  name: createdAt
  type: string
- description: ''
  name: description
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-hub-dataset-summary-schema.json
slug: hugging-face-hub-dataset-summary
source_filename: hugging-face-hub-dataset-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatasetSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset repository ID\"\n    },\n    \"author\": {\n      \"type\": \"string\"\n    },\n    \"sha\": {\n      \"type\": \"string\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\"\n    },\n    \"private\": {\n      \"type\": \"boolean\"\n    },\n    \"gated\": {\n      \"type\": \"boolean\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"downloads\": {\n      \"type\": \"integer\"\n    },\n    \"likes\": {\n      \"type\": \"integer\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-hub-dataset-summary-schema.json
tags: []
title: DatasetSummary
---
