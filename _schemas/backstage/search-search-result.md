---
description: SearchResult schema from Backstage search API
layout: schema
name: SearchResult
properties_list:
- description: The document type (e.g., software-catalog, techdocs).
  name: type
  type: string
- description: ''
  name: document
  type: object
- description: Relevance rank of the result.
  name: rank
  type: number
- description: ''
  name: highlight
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/search-search-result-schema.json
slug: search-search-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/search-search-result-schema.json\",\n  \"title\": \"SearchResult\",\n  \"description\": \"SearchResult schema from Backstage search API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The document type (e.g., software-catalog, techdocs).\"\n    },\n    \"document\": {\n      \"$ref\": \"#/components/schemas/SearchDocument\"\n    },\n    \"rank\": {\n      \"type\": \"number\",\n      \"description\": \"Relevance rank of the result.\"\n    },\n    \"highlight\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"preTag\": {\n          \"type\": \"string\"\n        },\n        \"postTag\": {\n          \"type\": \"string\"\n        },\n        \"fields\": {\n          \"type\": \"object\",\n          \"additionalProperties\"\
  : {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/search-search-result-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: SearchResult
---
