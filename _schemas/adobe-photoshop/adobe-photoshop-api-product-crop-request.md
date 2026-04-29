---
description: ProductCropRequest from Adobe Photoshop API
layout: schema
name: ProductCropRequest
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
schema_file: json-schema/adobe-photoshop-api-product-crop-request-schema.json
slug: adobe-photoshop-api-product-crop-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-product-crop-request-schema.json\",\n  \"title\": \"ProductCropRequest\",\n  \"description\": \"ProductCropRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageInput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"padding\": {\n          \"type\": \"number\",\n          \"description\": \"Padding around the product subject.\"\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"pixel\",\n            \"percent\"\n          ],\n          \"description\": \"Unit for padding value.\"\n        }\n      }\n    },\n    \"outputs\": {\n      \"\
  type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-product-crop-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: ProductCropRequest
---
