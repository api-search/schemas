---
description: A data source connection configured in Alation
layout: schema
name: DataSource
properties_list:
- description: Unique identifier
  name: id
  type: integer
- description: Display title
  name: title
  type: string
- description: Data source description
  name: description
  type: string
- description: Database type
  name: dbtype
  type: string
- description: Database host
  name: host
  type: string
- description: Database port
  name: port
  type: integer
- description: Virtual data source flag
  name: is_virtual
  type: boolean
- description: Catalog URL
  name: url
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-data-catalog-data-source-schema.json
slug: alation-alation-data-catalog-data-source
source_filename: alation-alation-data-catalog-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-data-catalog-data-source-schema.json\",\n  \"title\": \"DataSource\",\n  \"description\": \"A data source connection configured in Alation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Data source description\"\n    },\n    \"dbtype\": {\n      \"type\": \"string\",\n      \"description\": \"Database type\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Database host\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Database port\"\n    },\n    \"is_virtual\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Virtual data source flag\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Catalog URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-data-catalog-data-source-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: DataSource
---
