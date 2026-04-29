---
description: StorageOutput from Adobe Photoshop API
layout: schema
name: StorageOutput
properties_list:
- description: Pre-signed PUT URL or Creative Cloud asset path.
  name: href
  type: string
- description: Storage type for the output file.
  name: storage
  type: string
- description: Output file format.
  name: type
  type: string
- description: Optional output width in pixels for resizing.
  name: width
  type: integer
- description: Whether to overwrite existing files.
  name: overwrite
  type: boolean
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-storage-output-schema.json
slug: adobe-photoshop-api-storage-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-storage-output-schema.json\",\n  \"title\": \"StorageOutput\",\n  \"description\": \"StorageOutput from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"Pre-signed PUT URL or Creative Cloud asset path.\",\n      \"example\": \"https://image.adobe.io/example\"\n    },\n    \"storage\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"external\",\n        \"adobe\",\n        \"azure\",\n        \"dropbox\"\n      ],\n      \"description\": \"Storage type for the output file.\",\n      \"example\": \"external\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"image/jpeg\",\n        \"image/png\",\n        \"image/tiff\",\n        \"vnd.adobe.photoshop\"\
  \n      ],\n      \"description\": \"Output file format.\",\n      \"example\": \"image/jpeg\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Optional output width in pixels for resizing.\",\n      \"example\": 1920\n    },\n    \"overwrite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to overwrite existing files.\",\n      \"default\": true,\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"href\",\n    \"storage\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-storage-output-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: StorageOutput
---
