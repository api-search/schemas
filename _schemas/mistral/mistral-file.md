---
description: A file uploaded to the Mistral AI platform for use with fine-tuning, batch processing, or OCR endpoints.
layout: schema
name: Mistral File
properties_list:
- description: Unique identifier for the file
  name: id
  type: string
- description: Object type identifier
  name: object
  type: string
- description: File size in bytes
  name: bytes
  type: integer
- description: Unix timestamp when the file was uploaded
  name: created_at
  type: integer
- description: Original filename of the uploaded file
  name: filename
  type: string
- description: Intended purpose of the file
  name: purpose
  type: string
- description: Number of lines in the file for JSONL files
  name: num_lines
  type:
  - integer
  - 'null'
- description: How the file was created on the platform
  name: source
  type: string
provider_name: Mistral AI
provider_slug: mistral
schema_file: json-schema/mistral-file-schema.json
slug: mistral-file
source_filename: mistral-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.mistral.ai/schemas/mistral/file.json\",\n  \"title\": \"Mistral File\",\n  \"description\": \"A file uploaded to the Mistral AI platform for use with fine-tuning, batch processing, or OCR endpoints.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"object\", \"bytes\", \"created_at\", \"filename\", \"purpose\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the file\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\"file\"],\n      \"description\": \"Object type identifier\"\n    },\n    \"bytes\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"File size in bytes\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the file was uploaded\"\n    },\n    \"filename\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Original filename of the uploaded file\"\n    },\n    \"purpose\": {\n      \"type\": \"string\",\n      \"enum\": [\"fine-tune\", \"batch\", \"ocr\"],\n      \"description\": \"Intended purpose of the file\"\n    },\n    \"num_lines\": {\n      \"type\": [\"integer\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"Number of lines in the file for JSONL files\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"enum\": [\"upload\", \"repository\"],\n      \"description\": \"How the file was created on the platform\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/json-schema/mistral-file-schema.json
tags: []
title: Mistral File
---
