---
description: ''
layout: schema
name: PAIdentifier
properties_list:
- description: User's FactSet account path OR benchmark.
  name: id
  type: string
- description: Holdings Mode can be B&H, TBR, OMS, EXT or VLT.
  name: holdingsmode
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-pa-identifier-schema.json
slug: factset-pa-engine-pa-identifier
source_filename: factset-pa-engine-pa-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PAIdentifier\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"User's FactSet account path OR benchmark.\"\n    },\n    \"holdingsmode\": {\n      \"type\": \"string\",\n      \"description\": \"Holdings Mode can be B&H, TBR, OMS, EXT or VLT.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-pa-identifier-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PAIdentifier
---
