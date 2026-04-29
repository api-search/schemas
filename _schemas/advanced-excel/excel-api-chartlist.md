---
description: List of charts.
layout: schema
name: ChartList
properties_list:
- description: Array of charts.
  name: value
  type: array
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-chartlist-schema.json
slug: excel-api-chartlist
source_filename: excel-api-chartlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChartList\",\n  \"description\": \"List of charts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"Array of charts.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Chart\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-chartlist-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: ChartList
---
