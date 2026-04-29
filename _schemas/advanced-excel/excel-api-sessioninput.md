---
description: Request to create a workbook session.
layout: schema
name: SessionInput
properties_list:
- description: Whether changes should be persisted.
  name: persistChanges
  type: boolean
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-sessioninput-schema.json
slug: excel-api-sessioninput
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SessionInput\",\n  \"description\": \"Request to create a workbook session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"persistChanges\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether changes should be persisted.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-sessioninput-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: SessionInput
---
