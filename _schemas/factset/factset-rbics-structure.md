---
description: ''
layout: schema
name: structure
properties_list:
- description: RBICS Code for the classification.
  name: rbicsId
  type: string
- description: First date of the classification.
  name: firstDate
  type: string
- description: Date when the classification became no longer valid. If `null`, the classification is still valid.
  name: lastDate
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-rbics-structure-schema.json
slug: factset-rbics-structure
source_filename: factset-rbics-structure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"structure\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rbicsId\": {\n      \"type\": \"string\",\n      \"description\": \"RBICS Code for the classification.\"\n    },\n    \"firstDate\": {\n      \"type\": \"string\",\n      \"description\": \"First date of the classification.\"\n    },\n    \"lastDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date when the classification became no longer valid. If `null`, the classification is still valid.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-rbics-structure-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: structure
---
