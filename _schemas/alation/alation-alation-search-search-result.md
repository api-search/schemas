---
description: A search result from the Alation catalog
layout: schema
name: SearchResult
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: object_type
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: score
  type: number
- description: ''
  name: breadcrumb
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-search-search-result-schema.json
slug: alation-alation-search-search-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-search-search-result-schema.json\",\n  \"title\": \"SearchResult\",\n  \"description\": \"A search result from the Alation catalog\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"object_type\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"score\": {\n      \"type\": \"number\"\n    },\n    \"breadcrumb\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-search-search-result-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: SearchResult
---
