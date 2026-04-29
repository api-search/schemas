---
description: Request body for generating an object composite in a scene
layout: schema
name: ObjectCompositeRequest
properties_list:
- description: Text description of the object to generate and composite
  name: prompt
  type: string
- description: Text describing what to avoid in the generated object
  name: negativePrompt
  type: string
- description: ''
  name: contentClass
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
schema_file: json-schema/adobe-creative-suite-firefly-object-composite-request-schema.json
slug: adobe-creative-suite-firefly-object-composite-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-object-composite-request-schema.json\",\n  \"title\": \"ObjectCompositeRequest\",\n  \"description\": \"Request body for generating an object composite in a scene\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text description of the object to generate and composite\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    },\n    \"negativePrompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text describing what to avoid in the generated object\",\n      \"maxLength\": 1024,\n      \"example\": \"example_value\"\n    },\n    \"contentClass\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"photo\",\n        \"art\"\n      ],\n      \"example\": \"photo\"\
  \n    },\n    \"image\": {\n      \"$ref\": \"#/components/schemas/InputImageReference\"\n    },\n    \"mask\": {\n      \"$ref\": \"#/components/schemas/InputImageReference\"\n    },\n    \"numVariations\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"default\": 1,\n      \"example\": 1920\n    },\n    \"seeds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"required\": [\n    \"prompt\",\n    \"image\",\n    \"mask\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-object-composite-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: ObjectCompositeRequest
---
