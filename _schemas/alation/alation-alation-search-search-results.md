---
description: Collection of search results
layout: schema
name: SearchResults
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: results
  type: array
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-search-search-results-schema.json
slug: alation-alation-search-search-results
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-search-search-results-schema.json\",\n  \"title\": \"SearchResults\",\n  \"description\": \"Collection of search results\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-search-search-results-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: SearchResults
---
