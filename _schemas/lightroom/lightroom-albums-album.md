---
description: ''
layout: schema
name: Album
properties_list:
- description: Album unique identifier
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: Album subtype
  name: subtype
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-albums-album-schema.json
slug: lightroom-albums-album
source_filename: lightroom-albums-album-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Album\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Album unique identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Album subtype\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    },\n    \"updated\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-albums-album-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: Album
---
