---
description: Represents a row in an Excel table.
layout: schema
name: TableRow
properties_list:
- description: Zero-based index of the row.
  name: index
  type: integer
- description: Raw values of the row.
  name: values
  type: array
provider_name: Microsoft Excel
provider_slug: microsoft-excel
schema_file: json-schema/excel-graph-api-table-row-schema.json
slug: excel-graph-api-table-row
source_filename: excel-graph-api-table-row-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-table-row-schema.json\",\n  \"title\": \"TableRow\",\n  \"description\": \"Represents a row in an Excel table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Zero-based index of the row.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"Raw values of the row.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-table-row-schema.json
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
title: TableRow
---
