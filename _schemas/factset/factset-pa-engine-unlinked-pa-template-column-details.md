---
description: ''
layout: schema
name: UnlinkedPATemplateColumnDetails
properties_list:
- description: Unlinked template column name
  name: name
  type: string
- description: FactSet-defined or User-defined Column identifier.
  name: id
  type: string
- description: Column Statistic identifier
  name: statistics
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-unlinked-pa-template-column-details-schema.json
slug: factset-pa-engine-unlinked-pa-template-column-details
source_filename: factset-pa-engine-unlinked-pa-template-column-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UnlinkedPATemplateColumnDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unlinked template column name\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet-defined or User-defined Column identifier.\"\n    },\n    \"statistics\": {\n      \"type\": \"array\",\n      \"description\": \"Column Statistic identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-unlinked-pa-template-column-details-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: UnlinkedPATemplateColumnDetails
---
