---
description: Response wrapper for a single stock file metadata request
layout: schema
name: StockFileResponse
properties_list:
- description: Array containing the requested file (always contains one item)
  name: files
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-stock-file-response-schema.json
slug: adobe-creative-suite-stock-stock-file-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-stock-file-response-schema.json\",\n  \"title\": \"StockFileResponse\",\n  \"description\": \"Response wrapper for a single stock file metadata request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"Array containing the requested file (always contains one item)\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StockFile\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-stock-file-response-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: StockFileResponse
---
