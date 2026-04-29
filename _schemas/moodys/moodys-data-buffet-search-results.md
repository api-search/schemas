---
description: Paginated search results for series queries.
layout: schema
name: SearchResults
properties_list:
- description: Total number of matching series across all pages.
  name: totalCount
  type: integer
- description: The current pagination offset.
  name: offset
  type: integer
- description: The maximum results per page.
  name: limit
  type: integer
- description: Array of matching series metadata.
  name: results
  type: array
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-search-results-schema.json
slug: moodys-data-buffet-search-results
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResults\",\n  \"type\": \"object\",\n  \"description\": \"Paginated search results for series queries.\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching series across all pages.\"\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"The current pagination offset.\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum results per page.\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of matching series metadata.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-search-results-schema.json
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
title: SearchResults
---
