---
description: Request body for text-to-image generation
layout: schema
name: ImageGenerateRequest
properties_list:
- description: Text description of the image to generate
  name: prompt
  type: string
- description: Text description of elements to avoid in the generated image
  name: negativePrompt
  type: string
- description: Broad content category to guide the generation model
  name: contentClass
  type: string
- description: Number of image variations to generate (1 to 4)
  name: numVariations
  type: integer
- description: ''
  name: size
  type: object
- description: ''
  name: style
  type: object
- description: Array of integer seed values for reproducible generation. Providing the same seed with the same prompt produces the same output.
  name: seeds
  type: array
- description: BCP 47 language locale for prompt interpretation
  name: locale
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-firefly-image-generate-request-schema.json
slug: adobe-creative-suite-firefly-image-generate-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-image-generate-request-schema.json\",\n  \"title\": \"ImageGenerateRequest\",\n  \"description\": \"Request body for text-to-image generation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text description of the image to generate\",\n      \"maxLength\": 1024,\n      \"example\": \"A serene mountain lake at golden hour with reflections of pine trees\"\n    },\n    \"negativePrompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text description of elements to avoid in the generated image\",\n      \"maxLength\": 1024,\n      \"example\": \"blurry, low quality, distorted\"\n    },\n    \"contentClass\": {\n      \"type\": \"string\",\n      \"description\": \"Broad content category\
  \ to guide the generation model\",\n      \"enum\": [\n        \"photo\",\n        \"art\"\n      ],\n      \"example\": \"photo\"\n    },\n    \"numVariations\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of image variations to generate (1 to 4)\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"default\": 1,\n      \"example\": 2\n    },\n    \"size\": {\n      \"$ref\": \"#/components/schemas/ImageSize\"\n    },\n    \"style\": {\n      \"$ref\": \"#/components/schemas/StyleOptions\"\n    },\n    \"seeds\": {\n      \"type\": \"array\",\n      \"description\": \"Array of integer seed values for reproducible generation. Providing the same seed with the same prompt produces the same output.\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        42,\n        1337\n      ]\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"BCP 47 language locale for prompt interpretation\",\n      \"example\"\
  : \"en-US\"\n    }\n  },\n  \"required\": [\n    \"prompt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-firefly-image-generate-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: ImageGenerateRequest
---
