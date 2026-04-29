---
description: A cell range in a worksheet with values and formulas.
layout: schema
name: Range
properties_list:
- description: A1-style range address.
  name: address
  type: string
- description: 2D array of cell values.
  name: values
  type: array
- description: 2D array of cell formulas.
  name: formulas
  type: array
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-range-schema.json
slug: excel-api-range
source_filename: excel-api-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Range\",\n  \"description\": \"A cell range in a worksheet with values and formulas.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"A1-style range address.\",\n      \"example\": \"Sheet1!A1:B10\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"2D array of cell values.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"formulas\": {\n      \"type\": \"array\",\n      \"description\": \"2D array of cell formulas.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-range-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: Range
---
