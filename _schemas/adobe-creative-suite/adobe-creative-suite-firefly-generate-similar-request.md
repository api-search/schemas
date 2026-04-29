---
description: Request body for generating images similar to a reference image
layout: schema
name: GenerateSimilarRequest
properties_list:
- description: Optional text prompt to further guide the style or content
  name: prompt
  type: string
- description: ''
  name: image
  type: object
- description: ''
  name: numVariations
  type: integer
- description: ''
  name: size
  type: object
- description: ''
  name: seeds
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-generate-similar-request-schema.json
slug: adobe-creative-suite-firefly-generate-similar-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-generate-similar-request-schema.json\",\n  \"title\": \"GenerateSimilarRequest\",\n  \"description\": \"Request body for generating images similar to a reference image\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Optional text prompt to further guide the style or content\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    },\n    \"image\": {\n      \"$ref\": \"#/components/schemas/InputImageReference\"\n    },\n    \"numVariations\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"default\": 1,\n      \"example\": 1920\n    },\n    \"size\": {\n      \"$ref\": \"#/components/schemas/ImageSize\"\n    },\n    \"seeds\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"required\": [\n    \"image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-generate-similar-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: GenerateSimilarRequest
---
