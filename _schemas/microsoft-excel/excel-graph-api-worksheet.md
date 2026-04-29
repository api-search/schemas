---
description: Represents an Excel worksheet.
layout: schema
name: Worksheet
properties_list:
- description: Unique identifier for the worksheet.
  name: id
  type: string
- description: The display name of the worksheet.
  name: name
  type: string
- description: The zero-based position of the worksheet.
  name: position
  type: integer
- description: Worksheet visibility.
  name: visibility
  type: string
provider_name: Microsoft Excel
provider_slug: microsoft-excel
schema_file: json-schema/excel-graph-api-worksheet-schema.json
slug: excel-graph-api-worksheet
source_filename: excel-graph-api-worksheet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-worksheet-schema.json\",\n  \"title\": \"Worksheet\",\n  \"description\": \"Represents an Excel worksheet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the worksheet.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the worksheet.\"\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"The zero-based position of the worksheet.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Worksheet visibility.\",\n      \"enum\": [\"Visible\", \"Hidden\", \"VeryHidden\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-worksheet-schema.json
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
title: Worksheet
---
