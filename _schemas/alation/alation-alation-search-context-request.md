---
description: Request for aggregated catalog context
layout: schema
name: ContextRequest
properties_list:
- description: ''
  name: query
  type: string
- description: ''
  name: object_types
  type: array
- description: ''
  name: limit
  type: integer
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-search-context-request-schema.json
slug: alation-alation-search-context-request
source_filename: alation-alation-search-context-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-search-context-request-schema.json\",\n  \"title\": \"ContextRequest\",\n  \"description\": \"Request for aggregated catalog context\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\"\n    },\n    \"object_types\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-search-context-request-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: ContextRequest
---
