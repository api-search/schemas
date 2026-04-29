---
description: FillImageRequest from Adobe API
layout: schema
name: FillImageRequest
properties_list:
- description: ''
  name: image
  type: object
- description: ''
  name: mask
  type: object
- description: Text describing what to generate in the masked region.
  name: prompt
  type: string
- description: ''
  name: numVariations
  type: integer
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-firefly-api-fill-image-request-schema.json
slug: adobe-firefly-api-fill-image-request
source_filename: adobe-firefly-api-fill-image-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-fill-image-request-schema.json\",\n  \"title\": \"FillImageRequest\",\n  \"description\": \"FillImageRequest from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"$ref\": \"#/components/schemas/ImageReference\"\n    },\n    \"mask\": {\n      \"$ref\": \"#/components/schemas/ImageReference\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text describing what to generate in the masked region.\",\n      \"example\": \"A beautiful sunset over the ocean\"\n    },\n    \"numVariations\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"default\": 1,\n      \"example\": 42\n    }\n  },\n  \"required\": [\n    \"image\",\n    \"mask\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-fill-image-request-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: FillImageRequest
---
