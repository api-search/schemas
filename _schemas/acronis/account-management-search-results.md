---
description: Search results containing matching tenants and users
layout: schema
name: SearchResults
properties_list:
- description: ''
  name: items
  type: array
- description: Total number of results
  name: size
  type: integer
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-search-results-schema.json
slug: account-management-search-results
source_filename: account-management-search-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-search-results-schema.json\",\n  \"title\": \"SearchResults\",\n  \"description\": \"Search results containing matching tenants and users\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"additionalProperties\": true\n      }\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-search-results-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: SearchResults
---
