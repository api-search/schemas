---
description: FillMaskedAreasRequest from Adobe Photoshop API
layout: schema
name: FillMaskedAreasRequest
properties_list:
- description: ''
  name: image
  type: object
- description: ''
  name: masks
  type: array
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-fill-masked-areas-request-schema.json
slug: adobe-photoshop-api-fill-masked-areas-request
source_filename: adobe-photoshop-api-fill-masked-areas-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-fill-masked-areas-request-schema.json\",\n  \"title\": \"FillMaskedAreasRequest\",\n  \"description\": \"FillMaskedAreasRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"source\"\n      ],\n      \"properties\": {\n        \"source\": {\n          \"type\": \"object\",\n          \"required\": [\n            \"url\"\n          ],\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n              \"description\": \"Pre-signed URL of the source image.\"\n            }\n          }\n        }\n      }\n    },\n    \"masks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n      \
  \    \"source\"\n        ],\n        \"properties\": {\n          \"source\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"url\"\n            ],\n            \"properties\": {\n              \"url\": {\n                \"type\": \"string\",\n                \"description\": \"Pre-signed URL of the mask image.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"image\",\n    \"masks\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-fill-masked-areas-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: FillMaskedAreasRequest
---
