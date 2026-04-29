---
description: ExpandImageRequest from Adobe API
layout: schema
name: ExpandImageRequest
properties_list:
- description: ''
  name: image
  type: object
- description: ''
  name: size
  type: object
- description: Text describing the content to generate in expanded areas.
  name: prompt
  type: string
- description: How to position the original image within the expanded canvas.
  name: placement
  type: object
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-firefly-api-expand-image-request-schema.json
slug: adobe-firefly-api-expand-image-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-expand-image-request-schema.json\",\n  \"title\": \"ExpandImageRequest\",\n  \"description\": \"ExpandImageRequest from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image\": {\n      \"$ref\": \"#/components/schemas/ImageReference\"\n    },\n    \"size\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"width\",\n        \"height\"\n      ],\n      \"properties\": {\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"Target width in pixels.\"\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"Target height in pixels.\"\n        }\n      }\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text describing the content to generate in expanded\
  \ areas.\",\n      \"example\": \"A beautiful sunset over the ocean\"\n    },\n    \"placement\": {\n      \"type\": \"object\",\n      \"description\": \"How to position the original image within the expanded canvas.\",\n      \"properties\": {\n        \"alignment\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"horizontal\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"left\",\n                \"center\",\n                \"right\"\n              ]\n            },\n            \"vertical\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"top\",\n                \"center\",\n                \"bottom\"\n              ]\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"image\",\n    \"size\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-firefly-api-expand-image-request-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: ExpandImageRequest
---
