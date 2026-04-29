---
description: ''
layout: schema
name: SpaceSummary
properties_list:
- description: ''
  name: _id
  type: string
- description: Space repository ID
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
  name: tags
  type: array
- description: ''
  name: likes
  type: integer
- description: SDK used by the Space
  name: sdk
  type: string
- description: ''
  name: runtime
  type: object
- description: ''
  name: createdAt
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-hub-space-summary-schema.json
slug: hugging-face-hub-space-summary
source_filename: hugging-face-hub-space-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpaceSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Space repository ID\"\n    },\n    \"author\": {\n      \"type\": \"string\"\n    },\n    \"sha\": {\n      \"type\": \"string\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\"\n    },\n    \"private\": {\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"likes\": {\n      \"type\": \"integer\"\n    },\n    \"sdk\": {\n      \"type\": \"string\",\n      \"description\": \"SDK used by the Space\"\n    },\n    \"runtime\": {\n      \"type\": \"object\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-hub-space-summary-schema.json
tags: []
title: SpaceSummary
---
