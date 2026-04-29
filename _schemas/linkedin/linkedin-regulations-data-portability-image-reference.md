---
description: ImageReference from LinkedIn API
layout: schema
name: ImageReference
properties_list:
- description: ''
  name: cropped
  type: object
- description: ''
  name: original
  type: object
- description: ''
  name: cropInfo
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-image-reference-schema.json
slug: linkedin-regulations-data-portability-image-reference
source_filename: linkedin-regulations-data-portability-image-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-image-reference-schema.json\",\n  \"title\": \"ImageReference\",\n  \"description\": \"ImageReference from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cropped\": {\n      \"$ref\": \"#/components/schemas/ImageAsset\"\n    },\n    \"original\": {\n      \"$ref\": \"#/components/schemas/ImageAsset\"\n    },\n    \"cropInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"x\": {\n          \"type\": \"integer\",\n          \"example\": 0\n        },\n        \"y\": {\n          \"type\": \"integer\",\n          \"example\": 0\n        },\n        \"width\": {\n          \"type\": \"integer\",\n          \"example\": 400\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"example\": 400\n        }\n \
  \     }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-image-reference-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ImageReference
---
