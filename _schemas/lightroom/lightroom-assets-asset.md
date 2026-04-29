---
description: ''
layout: schema
name: Asset
properties_list:
- description: Asset unique identifier
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: subtype
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: ''
  name: revision_ids
  type: array
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-assets-asset-schema.json
slug: lightroom-assets-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Asset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Asset unique identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"subtype\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    },\n    \"updated\": {\n      \"type\": \"string\"\n    },\n    \"revision_ids\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-assets-asset-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: Asset
---
