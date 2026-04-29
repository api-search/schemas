---
description: Represents an Excel table.
layout: schema
name: Table
properties_list:
- description: Unique identifier for the table.
  name: id
  type: string
- description: The name of the table.
  name: name
  type: string
- description: Whether the header row is visible.
  name: showHeaders
  type: boolean
- description: Whether the total row is visible.
  name: showTotals
  type: boolean
- description: Table style name.
  name: style
  type: string
provider_name: Microsoft Excel
provider_slug: microsoft-excel
schema_file: json-schema/excel-graph-api-table-schema.json
slug: excel-graph-api-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-table-schema.json\",\n  \"title\": \"Table\",\n  \"description\": \"Represents an Excel table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the table.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table.\"\n    },\n    \"showHeaders\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the header row is visible.\"\n    },\n    \"showTotals\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the total row is visible.\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"Table style name.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-table-schema.json
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
title: Table
---
