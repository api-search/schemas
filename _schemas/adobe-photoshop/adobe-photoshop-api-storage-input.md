---
description: StorageInput from Adobe Photoshop API
layout: schema
name: StorageInput
properties_list:
- description: Pre-signed GET URL or Creative Cloud asset path.
  name: href
  type: string
- description: Storage type for the input file.
  name: storage
  type: string
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-storage-input-schema.json
slug: adobe-photoshop-api-storage-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-storage-input-schema.json\",\n  \"title\": \"StorageInput\",\n  \"description\": \"StorageInput from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"Pre-signed GET URL or Creative Cloud asset path.\",\n      \"example\": \"https://image.adobe.io/example\"\n    },\n    \"storage\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"external\",\n        \"adobe\",\n        \"azure\",\n        \"dropbox\"\n      ],\n      \"description\": \"Storage type for the input file.\",\n      \"example\": \"external\"\n    }\n  },\n  \"required\": [\n    \"href\",\n    \"storage\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-storage-input-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: StorageInput
---
