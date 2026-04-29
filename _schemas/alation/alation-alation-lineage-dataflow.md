---
description: A dataflow object representing a lineage path
layout: schema
name: Dataflow
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: external_id
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: sources
  type: array
- description: ''
  name: targets
  type: array
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-lineage-dataflow-schema.json
slug: alation-alation-lineage-dataflow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-lineage-dataflow-schema.json\",\n  \"title\": \"Dataflow\",\n  \"description\": \"A dataflow object representing a lineage path\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"external_id\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"targets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-lineage-dataflow-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: Dataflow
---
