---
description: A database schema in the Alation catalog
layout: schema
name: Schema
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
- description: Parent data source ID
  name: ds_id
  type: integer
- description: ''
  name: url
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-data-catalog-schema-schema.json
slug: alation-alation-data-catalog-schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-data-catalog-schema-schema.json\",\n  \"title\": \"Schema\",\n  \"description\": \"A database schema in the Alation catalog\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"ds_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent data source ID\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-data-catalog-schema-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: Schema
---
