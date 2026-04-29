---
description: Reference to an input file stored in cloud storage
layout: schema
name: StorageInput
properties_list:
- description: URL or path to the input file. For Creative Cloud, use the asset path. For external storage, use the presigned URL.
  name: href
  type: string
- description: Storage type where the input file is located
  name: storage
  type: string
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-firefly-services-storage-input-schema.json
slug: lightroom-firefly-services-storage-input
source_filename: lightroom-firefly-services-storage-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageInput\",\n  \"type\": \"object\",\n  \"description\": \"Reference to an input file stored in cloud storage\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"URL or path to the input file. For Creative Cloud, use the asset path. For external storage, use the presigned URL.\"\n    },\n    \"storage\": {\n      \"type\": \"string\",\n      \"description\": \"Storage type where the input file is located\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-firefly-services-storage-input-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: StorageInput
---
