---
description: ''
layout: schema
name: SearchPageResponseSearchResult
properties_list:
- description: ''
  name: results
  type: array
- description: ''
  name: start
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: size
  type: integer
- description: ''
  name: totalSize
  type: integer
- description: ''
  name: cqlQuery
  type: string
- description: ''
  name: searchDuration
  type: integer
- description: ''
  name: archivedResultCount
  type: integer
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-search-search-page-response-search-result-schema.json
slug: atlassian-confluence-search-search-page-response-search-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchPageResponseSearchResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\"\n    },\n    \"start\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"size\": {\n      \"type\": \"integer\"\n    },\n    \"totalSize\": {\n      \"type\": \"integer\"\n    },\n    \"cqlQuery\": {\n      \"type\": \"string\"\n    },\n    \"searchDuration\": {\n      \"type\": \"integer\"\n    },\n    \"archivedResultCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-search-search-page-response-search-result-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: SearchPageResponseSearchResult
---
