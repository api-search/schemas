---
description: Represents an Excel chart object.
layout: schema
name: Chart
properties_list:
- description: Unique identifier for the chart.
  name: id
  type: string
- description: The name of the chart.
  name: name
  type: string
- description: Height in points.
  name: height
  type: number
- description: Width in points.
  name: width
  type: number
- description: Left position in points.
  name: left
  type: number
- description: Top position in points.
  name: top
  type: number
provider_name: Microsoft Excel
provider_slug: microsoft-excel
schema_file: json-schema/excel-graph-api-chart-schema.json
slug: excel-graph-api-chart
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-chart-schema.json\",\n  \"title\": \"Chart\",\n  \"description\": \"Represents an Excel chart object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the chart.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the chart.\"\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Height in points.\"\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Width in points.\"\n    },\n    \"left\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Left position in points.\"\n    },\n    \"top\": {\n      \"\
  type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Top position in points.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-chart-schema.json
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
title: Chart
---
