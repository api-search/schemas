---
description: ArtboardCreateRequest from Adobe Photoshop API
layout: schema
name: ArtboardCreateRequest
properties_list:
- description: ''
  name: options
  type: object
- description: ''
  name: outputs
  type: array
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-artboard-create-request-schema.json
slug: adobe-photoshop-api-artboard-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-artboard-create-request-schema.json\",\n  \"title\": \"ArtboardCreateRequest\",\n  \"description\": \"ArtboardCreateRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"options\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"artboards\"\n      ],\n      \"properties\": {\n        \"artboards\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Artboard name.\"\n              },\n              \"width\": {\n                \"type\": \"integer\",\n                \"description\": \"Artboard width in pixels.\"\n              },\n              \"height\": {\n\
  \                \"type\": \"integer\",\n                \"description\": \"Artboard height in pixels.\"\n              },\n              \"layers\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"$ref\": \"#/components/schemas/LayerOperation\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"options\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-artboard-create-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: ArtboardCreateRequest
---
