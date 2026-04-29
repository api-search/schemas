---
description: A File represents a stored file in the Appmixer file management system, which can be used by flows and components.
layout: schema
name: Appmixer File
properties_list:
- description: Unique identifier for the file.
  name: fileId
  type: string
- description: Original filename of the uploaded file.
  name: filename
  type: string
- description: File size in bytes.
  name: length
  type: integer
- description: MIME type of the file.
  name: contentType
  type: string
- description: Timestamp when the file was uploaded.
  name: createdAt
  type: string
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/file.json
slug: file
source_filename: file.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/appmixer/blob/main/json-schema/file.json\",\n  \"title\": \"Appmixer File\",\n  \"description\": \"A File represents a stored file in the Appmixer file management system, which can be used by flows and components.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the file.\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Original filename of the uploaded file.\"\n    },\n    \"length\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the file.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the file was uploaded.\"\
  \n    }\n  },\n  \"required\": [\"fileId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/json-schema/file.json
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer File
---
