---
description: TextEditRequest from Adobe Photoshop API
layout: schema
name: TextEditRequest
properties_list:
- description: ''
  name: inputs
  type: array
- description: ''
  name: options
  type: object
- description: ''
  name: outputs
  type: array
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-text-edit-request-schema.json
slug: adobe-photoshop-api-text-edit-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-text-edit-request-schema.json\",\n  \"title\": \"TextEditRequest\",\n  \"description\": \"TextEditRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageInput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"manageMissingFonts\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"fail\",\n            \"useDefault\"\n          ],\n          \"description\": \"Behavior when fonts are missing.\"\n        },\n        \"globalFont\": {\n          \"type\": \"string\",\n          \"description\": \"Fallback font name when using useDefault.\"\n        },\n        \"fonts\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"Custom fonts provided via URL.\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/StorageInput\"\n          }\n        },\n        \"layers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"name\",\n              \"text\"\n            ],\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Name of the text layer to edit.\"\n              },\n              \"text\": {\n                \"$ref\": \"#/components/schemas/TextContent\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"options\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-text-edit-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: TextEditRequest
---
