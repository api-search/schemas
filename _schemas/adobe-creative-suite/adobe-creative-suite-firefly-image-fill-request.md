---
description: Request body for generative fill operation
layout: schema
name: ImageFillRequest
properties_list:
- description: Text prompt describing what to fill in the masked area
  name: prompt
  type: string
- description: Text describing what to avoid in the filled area
  name: negativePrompt
  type: string
- description: ''
  name: image
  type: object
- description: ''
  name: mask
  type: object
- description: ''
  name: numVariations
  type: integer
- description: ''
  name: seeds
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-image-fill-request-schema.json
slug: adobe-creative-suite-firefly-image-fill-request
source_filename: adobe-creative-suite-firefly-image-fill-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-image-fill-request-schema.json\",\n  \"title\": \"ImageFillRequest\",\n  \"description\": \"Request body for generative fill operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text prompt describing what to fill in the masked area\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    },\n    \"negativePrompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text describing what to avoid in the filled area\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    },\n    \"image\": {\n      \"$ref\": \"#/components/schemas/InputImageReference\"\n    },\n    \"mask\": {\n      \"$ref\": \"#/components/schemas/InputImageReference\"\n    },\n    \"\
  numVariations\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"default\": 1,\n      \"example\": 1920\n    },\n    \"seeds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"required\": [\n    \"image\",\n    \"mask\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-image-fill-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: ImageFillRequest
---
