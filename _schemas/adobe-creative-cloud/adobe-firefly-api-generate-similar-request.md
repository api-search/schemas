---
description: GenerateSimilarRequest from Adobe API
layout: schema
name: GenerateSimilarRequest
properties_list:
- description: ''
  name: image
  type: object
- description: Optional text prompt to guide similar generation.
  name: prompt
  type: string
- description: ''
  name: numVariations
  type: integer
- description: ''
  name: size
  type: object
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-firefly-api-generate-similar-request-schema.json
slug: adobe-firefly-api-generate-similar-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-generate-similar-request-schema.json\",\n  \"title\": \"GenerateSimilarRequest\",\n  \"description\": \"GenerateSimilarRequest from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"$ref\": \"#/components/schemas/ImageReference\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Optional text prompt to guide similar generation.\",\n      \"example\": \"A beautiful sunset over the ocean\"\n    },\n    \"numVariations\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4,\n      \"default\": 1,\n      \"example\": 42\n    },\n    \"size\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"height\": {\n    \
  \      \"type\": \"integer\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"image\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-generate-similar-request-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: GenerateSimilarRequest
---
