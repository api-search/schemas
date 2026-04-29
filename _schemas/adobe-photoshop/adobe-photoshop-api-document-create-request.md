---
description: DocumentCreateRequest from Adobe Photoshop API
layout: schema
name: DocumentCreateRequest
properties_list:
- description: ''
  name: options
  type: object
- description: ''
  name: outputs
  type: array
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-document-create-request-schema.json
slug: adobe-photoshop-api-document-create-request
source_filename: adobe-photoshop-api-document-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-document-create-request-schema.json\",\n  \"title\": \"DocumentCreateRequest\",\n  \"description\": \"DocumentCreateRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"options\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"document\"\n      ],\n      \"properties\": {\n        \"document\": {\n          \"type\": \"object\",\n          \"required\": [\n            \"width\",\n            \"height\"\n          ],\n          \"properties\": {\n            \"width\": {\n              \"type\": \"integer\",\n              \"description\": \"Document width in pixels.\"\n            },\n            \"height\": {\n              \"type\": \"integer\",\n              \"description\": \"Document height in pixels.\"\n            },\n  \
  \          \"resolution\": {\n              \"type\": \"integer\",\n              \"default\": 72,\n              \"description\": \"Document resolution in PPI.\"\n            },\n            \"fill\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"white\",\n                \"transparent\",\n                \"backgroundColor\"\n              ],\n              \"default\": \"white\"\n            },\n            \"mode\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"rgb\",\n                \"cmyk\",\n                \"grayscale\"\n              ],\n              \"default\": \"rgb\"\n            },\n            \"depth\": {\n              \"type\": \"integer\",\n              \"enum\": [\n                8,\n                16,\n                32\n              ],\n              \"default\": 8,\n              \"description\": \"Bit depth per channel.\"\n            }\n          }\n        },\n        \"layers\"\
  : {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/LayerOperation\"\n          }\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"options\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-document-create-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: DocumentCreateRequest
---
