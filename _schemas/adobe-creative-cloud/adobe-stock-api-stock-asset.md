---
description: StockAsset from Adobe API
layout: schema
name: StockAsset
properties_list:
- description: Unique asset identifier.
  name: id
  type: integer
- description: ''
  name: title
  type: string
- description: ''
  name: creator_name
  type: string
- description: ''
  name: creator_id
  type: integer
- description: Asset type (photo, illustration, vector, video, template, 3d).
  name: content_type
  type: string
- description: ''
  name: width
  type: integer
- description: ''
  name: height
  type: integer
- description: ''
  name: thumbnail_url
  type: string
- description: ''
  name: thumbnail_width
  type: integer
- description: ''
  name: thumbnail_height
  type: integer
- description: URL to the watermarked comp/preview.
  name: comp_url
  type: string
- description: ''
  name: category
  type: object
- description: ''
  name: keywords
  type: array
- description: License type if already licensed, empty string if not.
  name: is_licensed
  type: string
- description: 0 = Core, 1 = Free, 2 = Premium Collection 1, 3 = Premium Collection 2.
  name: premium_level_id
  type: integer
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-stock-api-stock-asset-schema.json
slug: adobe-stock-api-stock-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-stock-asset-schema.json\",\n  \"title\": \"StockAsset\",\n  \"description\": \"StockAsset from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique asset identifier.\",\n      \"example\": 42\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"creator_name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Asset\"\n    },\n    \"creator_id\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"Asset type (photo, illustration, vector, video, template, 3d).\",\n      \"example\": \"image\"\n    },\n    \"width\": {\n      \"type\": \"integer\"\
  ,\n      \"example\": 42\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://example.adobe.com/asset\"\n    },\n    \"thumbnail_width\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"thumbnail_height\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"comp_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the watermarked comp/preview.\",\n      \"example\": \"https://example.adobe.com/asset\"\n    },\n    \"category\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n    \
  \      \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"is_licensed\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Standard\",\n        \"Extended\",\n        \"Video_HD\",\n        \"Video_4K\",\n        \"\"\n      ],\n      \"description\": \"License type if already licensed, empty string if not.\",\n      \"example\": \"Standard\"\n    },\n    \"premium_level_id\": {\n      \"type\": \"integer\",\n      \"description\": \"0 = Core, 1 = Free, 2 = Premium Collection 1, 3 = Premium Collection 2.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-stock-asset-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: StockAsset
---
