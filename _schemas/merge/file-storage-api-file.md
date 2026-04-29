---
description: A file object from a connected file storage platform.
layout: schema
name: File
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: remote_id
  type: string
- description: File name.
  name: name
  type: string
- description: ''
  name: file_url
  type: string
- description: ''
  name: file_thumbnail_url
  type: string
- description: File size in bytes.
  name: size
  type: integer
- description: ''
  name: mime_type
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: folder
  type: string
- description: ''
  name: drive
  type: string
- description: ''
  name: remote_was_deleted
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: modified_at
  type: string
provider_name: Merge
provider_slug: merge
schema_file: json-schema/file-storage-api-file-schema.json
slug: file-storage-api-file
source_filename: file-storage-api-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/file-storage-api-file-schema.json\",\n  \"title\": \"File\",\n  \"description\": \"A file object from a connected file storage platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"remote_id\": { \"type\": \"string\" },\n    \"name\": { \"type\": \"string\", \"description\": \"File name.\" },\n    \"file_url\": { \"type\": \"string\", \"format\": \"uri\" },\n    \"file_thumbnail_url\": { \"type\": \"string\", \"format\": \"uri\" },\n    \"size\": { \"type\": \"integer\", \"description\": \"File size in bytes.\" },\n    \"mime_type\": { \"type\": \"string\" },\n    \"description\": { \"type\": \"string\" },\n    \"folder\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"drive\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"\
  remote_was_deleted\": { \"type\": \"boolean\" },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"modified_at\": { \"type\": \"string\", \"format\": \"date-time\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/file-storage-api-file-schema.json
tags:
- Integrations
- Platform
- Unified API
title: File
---
