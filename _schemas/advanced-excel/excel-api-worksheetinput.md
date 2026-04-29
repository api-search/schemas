---
description: Request to add a new worksheet.
layout: schema
name: WorksheetInput
properties_list:
- description: Name for the new worksheet.
  name: name
  type: string
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-worksheetinput-schema.json
slug: excel-api-worksheetinput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorksheetInput\",\n  \"description\": \"Request to add a new worksheet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new worksheet.\",\n      \"example\": \"Sales Data\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-worksheetinput-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: WorksheetInput
---
