---
description: Column settings (name, directory, category)
layout: schema
name: ColumnSummary
properties_list:
- description: Column Name
  name: name
  type: string
- description: Column Directory
  name: directory
  type: string
- description: Column Category
  name: category
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-pa-engine-column-summary-schema.json
slug: factset-pa-engine-column-summary
source_filename: factset-pa-engine-column-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColumnSummary\",\n  \"type\": \"object\",\n  \"description\": \"Column settings (name, directory, category)\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Column Name\"\n    },\n    \"directory\": {\n      \"type\": \"string\",\n      \"description\": \"Column Directory\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Column Category\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-pa-engine-column-summary-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: ColumnSummary
---
