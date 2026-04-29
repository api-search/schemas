---
description: A data quality rule for catalog objects
layout: schema
name: DataQualityRule
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: rule_type
  type: string
- description: ''
  name: object_type
  type: string
- description: ''
  name: object_id
  type: integer
- description: ''
  name: created_at
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-governance-data-quality-rule-schema.json
slug: alation-alation-governance-data-quality-rule
source_filename: alation-alation-governance-data-quality-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-governance-data-quality-rule-schema.json\",\n  \"title\": \"DataQualityRule\",\n  \"description\": \"A data quality rule for catalog objects\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"rule_type\": {\n      \"type\": \"string\"\n    },\n    \"object_type\": {\n      \"type\": \"string\"\n    },\n    \"object_id\": {\n      \"type\": \"integer\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-governance-data-quality-rule-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: DataQualityRule
---
