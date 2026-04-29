---
description: SearchResultSet schema from Backstage search API
layout: schema
name: SearchResultSet
properties_list:
- description: Array of search result documents.
  name: results
  type: array
- description: Cursor to fetch the next page of results.
  name: nextPageCursor
  type: string
- description: Cursor to fetch the previous page of results.
  name: previousPageCursor
  type: string
- description: Total number of matching results.
  name: numberOfResults
  type: integer
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/search-search-result-set-schema.json
slug: search-search-result-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/search-search-result-set-schema.json\",\n  \"title\": \"SearchResultSet\",\n  \"description\": \"SearchResultSet schema from Backstage search API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SearchResult\"\n      },\n      \"description\": \"Array of search result documents.\"\n    },\n    \"nextPageCursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor to fetch the next page of results.\"\n    },\n    \"previousPageCursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor to fetch the previous page of results.\"\n    },\n    \"numberOfResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/search-search-result-set-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: SearchResultSet
---
