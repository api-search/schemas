---
description: A database table in the Alation catalog
layout: schema
name: Table
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: schema_id
  type: integer
- description: ''
  name: ds_id
  type: integer
- description: ''
  name: table_type
  type: string
- description: ''
  name: url
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-data-catalog-table-schema.json
slug: alation-alation-data-catalog-table
source_filename: alation-alation-data-catalog-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-data-catalog-table-schema.json\",\n  \"title\": \"Table\",\n  \"description\": \"A database table in the Alation catalog\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"schema_id\": {\n      \"type\": \"integer\"\n    },\n    \"ds_id\": {\n      \"type\": \"integer\"\n    },\n    \"table_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TABLE\",\n        \"VIEW\",\n        \"EXTERNAL\"\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-data-catalog-table-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: Table
---
