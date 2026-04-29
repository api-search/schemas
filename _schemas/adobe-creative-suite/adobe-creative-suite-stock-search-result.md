---
description: Paginated search results from the Adobe Stock library
layout: schema
name: SearchResult
properties_list:
- description: Total number of files matching the search query
  name: nb_results
  type: integer
- description: List of matching stock files
  name: files
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-search-result-schema.json
slug: adobe-creative-suite-stock-search-result
source_filename: adobe-creative-suite-stock-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-search-result-schema.json\",\n  \"title\": \"SearchResult\",\n  \"description\": \"Paginated search results from the Adobe Stock library\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nb_results\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of files matching the search query\",\n      \"example\": 4521\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"List of matching stock files\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StockFile\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-search-result-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: SearchResult
---
