---
description: Represents a cell range in a worksheet.
layout: schema
name: Range
properties_list:
- description: Range reference in A1-style notation.
  name: address
  type: string
- description: Range reference in locale-specific notation.
  name: addressLocal
  type: string
- description: Number of cells in the range.
  name: cellCount
  type: integer
- description: Number of columns.
  name: columnCount
  type: integer
- description: Column number of the first cell.
  name: columnIndex
  type: integer
- description: Number of rows.
  name: rowCount
  type: integer
- description: Row number of the first cell.
  name: rowIndex
  type: integer
- description: Whether the range is hidden.
  name: hidden
  type: boolean
- description: Formulas in A1-style notation.
  name: formulas
  type: array
- description: Raw values of the range.
  name: values
  type: array
- description: Text values of the range.
  name: text
  type: array
- description: Number format codes.
  name: numberFormat
  type: array
- description: Type of data in each cell.
  name: valueTypes
  type: array
provider_name: Microsoft Excel
provider_slug: microsoft-excel
schema_file: json-schema/excel-graph-api-range-schema.json
slug: excel-graph-api-range
source_filename: excel-graph-api-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-range-schema.json\",\n  \"title\": \"Range\",\n  \"description\": \"Represents a cell range in a worksheet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Range reference in A1-style notation.\"\n    },\n    \"addressLocal\": {\n      \"type\": \"string\",\n      \"description\": \"Range reference in locale-specific notation.\"\n    },\n    \"cellCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of cells in the range.\"\n    },\n    \"columnCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of columns.\"\n    },\n    \"columnIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"Column number of the first cell.\"\n    },\n    \"rowCount\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Number of rows.\"\n    },\n    \"rowIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"Row number of the first cell.\"\n    },\n    \"hidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the range is hidden.\"\n    },\n    \"formulas\": {\n      \"type\": \"array\",\n      \"description\": \"Formulas in A1-style notation.\",\n      \"items\": { \"type\": \"array\", \"items\": {} }\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"Raw values of the range.\",\n      \"items\": { \"type\": \"array\", \"items\": {} }\n    },\n    \"text\": {\n      \"type\": \"array\",\n      \"description\": \"Text values of the range.\",\n      \"items\": { \"type\": \"array\", \"items\": {} }\n    },\n    \"numberFormat\": {\n      \"type\": \"array\",\n      \"description\": \"Number format codes.\",\n      \"items\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n    },\n    \"\
  valueTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Type of data in each cell.\",\n      \"items\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-range-schema.json
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
title: Range
---
