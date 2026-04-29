---
description: An Excel table.
layout: schema
name: Table
properties_list:
- description: Table identifier.
  name: id
  type: string
- description: Table name.
  name: name
  type: string
- description: Whether header row is shown.
  name: showHeaders
  type: boolean
- description: Whether total row is shown.
  name: showTotals
  type: boolean
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-table-schema.json
slug: excel-api-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Table\",\n  \"description\": \"An Excel table.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Table identifier.\",\n      \"example\": \"table1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Table name.\",\n      \"example\": \"SalesTable\"\n    },\n    \"showHeaders\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether header row is shown.\",\n      \"example\": true\n    },\n    \"showTotals\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether total row is shown.\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-table-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: Table
---
