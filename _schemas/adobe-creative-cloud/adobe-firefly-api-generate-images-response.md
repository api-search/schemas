---
description: GenerateImagesResponse from Adobe API
layout: schema
name: GenerateImagesResponse
properties_list:
- description: ''
  name: size
  type: object
- description: ''
  name: outputs
  type: array
- description: ''
  name: contentClass
  type: string
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-firefly-api-generate-images-response-schema.json
slug: adobe-firefly-api-generate-images-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-generate-images-response-schema.json\",\n  \"title\": \"GenerateImagesResponse\",\n  \"description\": \"GenerateImagesResponse from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"size\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"height\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"seed\": {\n            \"type\": \"integer\",\n            \"description\": \"Random seed used for this variation.\"\n          },\n          \"image\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"\
  url\": {\n                \"type\": \"string\",\n                \"format\": \"uri\",\n                \"description\": \"URL to the generated image. Expires after 24 hours.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"contentClass\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-generate-images-response-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: GenerateImagesResponse
---
