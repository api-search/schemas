---
description: ''
layout: schema
name: PACalculationGroup
properties_list:
- description: FactSet-defined or User-defined Group identifier.
  name: id
  type: string
- description: Grouping frequency
  name: frequency
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-pa-calculation-group-schema.json
slug: factset-pa-engine-pa-calculation-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PACalculationGroup\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet-defined or User-defined Group identifier.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Grouping frequency\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-pa-calculation-group-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PACalculationGroup
---
