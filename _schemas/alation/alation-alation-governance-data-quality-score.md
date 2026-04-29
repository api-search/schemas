---
description: Data quality scores for a catalog object
layout: schema
name: DataQualityScore
properties_list:
- description: ''
  name: object_type
  type: string
- description: ''
  name: object_id
  type: integer
- description: ''
  name: overall_score
  type: number
- description: ''
  name: dimensions
  type: object
- description: ''
  name: last_evaluated
  type: string
provider_name: Alation
provider_slug: alation
schema_file: json-schema/alation-alation-governance-data-quality-score-schema.json
slug: alation-alation-governance-data-quality-score
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-governance-data-quality-score-schema.json\",\n  \"title\": \"DataQualityScore\",\n  \"description\": \"Data quality scores for a catalog object\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object_type\": {\n      \"type\": \"string\"\n    },\n    \"object_id\": {\n      \"type\": \"integer\"\n    },\n    \"overall_score\": {\n      \"type\": \"number\"\n    },\n    \"dimensions\": {\n      \"type\": \"object\"\n    },\n    \"last_evaluated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/json-schema/alation-alation-governance-data-quality-score-schema.json
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
title: DataQualityScore
---
