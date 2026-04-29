---
description: List of worksheets.
layout: schema
name: WorksheetList
properties_list:
- description: Array of worksheets.
  name: value
  type: array
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-worksheetlist-schema.json
slug: excel-api-worksheetlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorksheetList\",\n  \"description\": \"List of worksheets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of worksheets.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Worksheet\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-worksheetlist-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: WorksheetList
---
