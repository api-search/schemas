---
description: An Excel worksheet.
layout: schema
name: Worksheet
properties_list:
- description: Worksheet identifier.
  name: id
  type: string
- description: Worksheet display name.
  name: name
  type: string
- description: Zero-based index position.
  name: position
  type: integer
- description: Visibility.
  name: visibility
  type: string
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-worksheet-schema.json
slug: excel-api-worksheet
source_filename: excel-api-worksheet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Worksheet\",\n  \"description\": \"An Excel worksheet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Worksheet identifier.\",\n      \"example\": \"sheet1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Worksheet display name.\",\n      \"example\": \"Sheet1\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"Zero-based index position.\",\n      \"example\": 0\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Visibility.\",\n      \"enum\": [\n        \"Visible\",\n        \"Hidden\",\n        \"VeryHidden\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-worksheet-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: Worksheet
---
