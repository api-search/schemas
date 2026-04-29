---
description: Paginated license history for the authenticated member
layout: schema
name: LicenseHistoryResult
properties_list:
- description: Total number of licensing events in the history
  name: nb_results
  type: integer
- description: List of previously licensed stock files
  name: files
  type: array
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-license-history-result-schema.json
slug: adobe-creative-suite-stock-license-history-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-history-result-schema.json\",\n  \"title\": \"LicenseHistoryResult\",\n  \"description\": \"Paginated license history for the authenticated member\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nb_results\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of licensing events in the history\",\n      \"example\": 87\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"List of previously licensed stock files\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StockFile\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-history-result-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: LicenseHistoryResult
---
