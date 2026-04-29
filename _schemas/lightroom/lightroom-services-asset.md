---
description: ''
layout: schema
name: Asset
properties_list:
- description: Unique identifier of the asset
  name: id
  type: string
- description: Resource type
  name: type
  type: string
- description: Asset subtype
  name: subtype
  type: string
- description: Asset creation timestamp
  name: created
  type: string
- description: Asset last updated timestamp
  name: updated
  type: string
- description: List of revision identifiers
  name: revision_ids
  type: array
- description: Asset payload containing metadata
  name: payload
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-services-asset-schema.json
slug: lightroom-services-asset
source_filename: lightroom-services-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Asset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the asset\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Asset subtype\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"Asset creation timestamp\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"description\": \"Asset last updated timestamp\"\n    },\n    \"revision_ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of revision identifiers\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Asset payload containing metadata\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-services-asset-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: Asset
---
