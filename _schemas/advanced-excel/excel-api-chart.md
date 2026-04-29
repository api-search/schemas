---
description: An Excel chart.
layout: schema
name: Chart
properties_list:
- description: Chart identifier.
  name: id
  type: string
- description: Chart name.
  name: name
  type: string
- description: Chart type.
  name: chartType
  type: string
- description: Height in points.
  name: height
  type: number
- description: Width in points.
  name: width
  type: number
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-chart-schema.json
slug: excel-api-chart
source_filename: excel-api-chart-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Chart\",\n  \"description\": \"An Excel chart.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Chart identifier.\",\n      \"example\": \"chart1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Chart name.\",\n      \"example\": \"SalesChart\"\n    },\n    \"chartType\": {\n      \"type\": \"string\",\n      \"description\": \"Chart type.\",\n      \"example\": \"ColumnClustered\"\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Height in points.\",\n      \"example\": 300\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Width in points.\",\n      \"example\": 500\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-chart-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: Chart
---
