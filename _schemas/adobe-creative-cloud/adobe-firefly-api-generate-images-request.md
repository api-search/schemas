---
description: GenerateImagesRequest from Adobe API
layout: schema
name: GenerateImagesRequest
properties_list:
- description: Text description of the image to generate.
  name: prompt
  type: string
- description: Text describing elements to exclude from generation.
  name: negativePrompt
  type: string
- description: Number of image variations to generate.
  name: numVariations
  type: integer
- description: Output image dimensions.
  name: size
  type: object
- description: Content class hint. photo optimizes for photorealistic output, art for artistic/illustrated styles.
  name: contentClass
  type: string
- description: Style configuration for generation.
  name: style
  type: object
- description: Random seeds for reproducible generation. One seed per requested variation.
  name: seeds
  type: array
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-firefly-api-generate-images-request-schema.json
slug: adobe-firefly-api-generate-images-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-generate-images-request-schema.json\",\n  \"title\": \"GenerateImagesRequest\",\n  \"description\": \"GenerateImagesRequest from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"maxLength\": 1024,\n      \"description\": \"Text description of the image to generate.\",\n      \"example\": \"A beautiful sunset over the ocean\"\n    },\n    \"negativePrompt\": {\n      \"type\": \"string\",\n      \"maxLength\": 1024,\n      \"description\": \"Text describing elements to exclude from generation.\",\n      \"example\": \"A beautiful sunset over the ocean\"\n    },\n    \"numVariations\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"default\": 1,\n      \"description\": \"Number\
  \ of image variations to generate.\",\n      \"example\": 42\n    },\n    \"size\": {\n      \"type\": \"object\",\n      \"description\": \"Output image dimensions.\",\n      \"properties\": {\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"Width in pixels.\"\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"Height in pixels.\"\n        }\n      }\n    },\n    \"contentClass\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"photo\",\n        \"art\"\n      ],\n      \"description\": \"Content class hint. photo optimizes for photorealistic output, art for artistic/illustrated styles.\",\n      \"example\": \"photo\"\n    },\n    \"style\": {\n      \"type\": \"object\",\n      \"description\": \"Style configuration for generation.\",\n      \"properties\": {\n        \"presets\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n\
  \          \"description\": \"Style preset identifiers.\"\n        },\n        \"referenceImage\": {\n          \"$ref\": \"#/components/schemas/ImageReference\"\n        }\n      }\n    },\n    \"seeds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"Random seeds for reproducible generation. One seed per requested variation.\"\n    }\n  },\n  \"required\": [\n    \"prompt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-generate-images-request-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: GenerateImagesRequest
---
