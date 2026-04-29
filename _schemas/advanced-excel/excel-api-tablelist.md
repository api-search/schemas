---
description: List of Excel tables.
layout: schema
name: TableList
properties_list:
- description: Array of tables.
  name: value
  type: array
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-tablelist-schema.json
slug: excel-api-tablelist
source_filename: excel-api-tablelist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableList\",\n  \"description\": \"List of Excel tables.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of tables.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Table\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-tablelist-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: TableList
---
