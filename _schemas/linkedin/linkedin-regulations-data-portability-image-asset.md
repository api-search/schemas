---
description: ImageAsset from LinkedIn API
layout: schema
name: ImageAsset
properties_list:
- description: ''
  name: downloadUrl
  type: string
- description: ''
  name: downloadUrlExpiresAt
  type: integer
- description: ''
  name: status
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-regulations-data-portability-image-asset-schema.json
slug: linkedin-regulations-data-portability-image-asset
source_filename: linkedin-regulations-data-portability-image-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-image-asset-schema.json\",\n  \"title\": \"ImageAsset\",\n  \"description\": \"ImageAsset from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://media.licdn.com/dms/image/...\"\n    },\n    \"downloadUrlExpiresAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1710979200000\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"PROCESSING\",\n        \"FAILED\"\n      ],\n      \"example\": \"AVAILABLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-regulations-data-portability-image-asset-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ImageAsset
---
