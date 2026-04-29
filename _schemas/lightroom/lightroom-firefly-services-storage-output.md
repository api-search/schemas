---
description: Reference to the output destination in cloud storage
layout: schema
name: StorageOutput
properties_list:
- description: URL or path for the output file
  name: href
  type: string
- description: Storage type for the output
  name: storage
  type: string
- description: Output image format
  name: type
  type: string
- description: Whether to overwrite existing files
  name: overwrite
  type: boolean
- description: JPEG quality (1-12) when output type is image/jpeg
  name: quality
  type: integer
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-firefly-services-storage-output-schema.json
slug: lightroom-firefly-services-storage-output
source_filename: lightroom-firefly-services-storage-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageOutput\",\n  \"type\": \"object\",\n  \"description\": \"Reference to the output destination in cloud storage\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"URL or path for the output file\"\n    },\n    \"storage\": {\n      \"type\": \"string\",\n      \"description\": \"Storage type for the output\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Output image format\"\n    },\n    \"overwrite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to overwrite existing files\"\n    },\n    \"quality\": {\n      \"type\": \"integer\",\n      \"description\": \"JPEG quality (1-12) when output type is image/jpeg\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-firefly-services-storage-output-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: StorageOutput
---
