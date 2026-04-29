---
description: Request body for generative image expansion
layout: schema
name: ImageExpandRequest
properties_list:
- description: Text prompt to guide what content fills the expanded areas
  name: prompt
  type: string
- description: Text describing what to avoid in the expanded areas
  name: negativePrompt
  type: string
- description: ''
  name: image
  type: object
- description: ''
  name: size
  type: object
- description: Placement and inset parameters for the source image within the expanded canvas
  name: placement
  type: object
- description: ''
  name: numVariations
  type: integer
- description: ''
  name: seeds
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-image-expand-request-schema.json
slug: adobe-creative-suite-firefly-image-expand-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-image-expand-request-schema.json\",\n  \"title\": \"ImageExpandRequest\",\n  \"description\": \"Request body for generative image expansion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text prompt to guide what content fills the expanded areas\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    },\n    \"negativePrompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text describing what to avoid in the expanded areas\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    },\n    \"image\": {\n      \"$ref\": \"#/components/schemas/InputImageReference\"\n    },\n    \"size\": {\n      \"$ref\": \"#/components/schemas/ImageSize\"\n    },\n  \
  \  \"placement\": {\n      \"type\": \"object\",\n      \"description\": \"Placement and inset parameters for the source image within the expanded canvas\",\n      \"properties\": {\n        \"inset\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"left\": {\n              \"type\": \"integer\"\n            },\n            \"top\": {\n              \"type\": \"integer\"\n            },\n            \"right\": {\n              \"type\": \"integer\"\n            },\n            \"bottom\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    },\n    \"numVariations\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"default\": 1,\n      \"example\": 1920\n    },\n    \"seeds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"required\": [\n    \"image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-image-expand-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: ImageExpandRequest
---
