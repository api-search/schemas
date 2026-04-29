---
description: Request to create a chart.
layout: schema
name: ChartInput
properties_list:
- description: Chart type.
  name: type
  type: string
- description: A1-style data range.
  name: sourceData
  type: string
- description: How series are plotted.
  name: seriesBy
  type: string
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-chartinput-schema.json
slug: excel-api-chartinput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChartInput\",\n  \"description\": \"Request to create a chart.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Chart type.\",\n      \"example\": \"ColumnClustered\"\n    },\n    \"sourceData\": {\n      \"type\": \"string\",\n      \"description\": \"A1-style data range.\",\n      \"example\": \"Sheet1!A1:B10\"\n    },\n    \"seriesBy\": {\n      \"type\": \"string\",\n      \"description\": \"How series are plotted.\",\n      \"enum\": [\n        \"Auto\",\n        \"Columns\",\n        \"Rows\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-chartinput-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: ChartInput
---
