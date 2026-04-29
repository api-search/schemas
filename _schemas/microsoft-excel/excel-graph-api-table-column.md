---
description: Represents a column in an Excel table.
layout: schema
name: TableColumn
properties_list:
- description: Unique identifier for the column.
  name: id
  type: string
- description: Zero-based index of the column.
  name: index
  type: integer
- description: The name of the column.
  name: name
  type: string
- description: Raw values of the column.
  name: values
  type: array
provider_name: Microsoft Excel
provider_slug: microsoft-excel
schema_file: json-schema/excel-graph-api-table-column-schema.json
slug: excel-graph-api-table-column
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-table-column-schema.json\",\n  \"title\": \"TableColumn\",\n  \"description\": \"Represents a column in an Excel table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the column.\"\n    },\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Zero-based index of the column.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the column.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"Raw values of the column.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-table-column-schema.json
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
title: TableColumn
---
