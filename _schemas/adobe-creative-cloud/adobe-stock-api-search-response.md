---
description: SearchResponse from Adobe API
layout: schema
name: SearchResponse
properties_list:
- description: Total number of matching results.
  name: nb_results
  type: integer
- description: ''
  name: files
  type: array
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
schema_file: json-schema/adobe-stock-api-search-response-schema.json
slug: adobe-stock-api-search-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-search-response-schema.json\",\n  \"title\": \"SearchResponse\",\n  \"description\": \"SearchResponse from Adobe API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nb_results\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching results.\",\n      \"example\": 42\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StockAsset\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/json-schema/adobe-stock-api-search-response-schema.json
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
title: SearchResponse
---
