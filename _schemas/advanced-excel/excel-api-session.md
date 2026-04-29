---
description: A workbook session for batch operations.
layout: schema
name: Session
properties_list:
- description: Session identifier.
  name: id
  type: string
- description: Whether changes are persisted.
  name: persistChanges
  type: boolean
provider_name: Advanced Excel
provider_slug: advanced-excel
schema_file: json-schema/excel-api-session-schema.json
slug: excel-api-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Session\",\n  \"description\": \"A workbook session for batch operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Session identifier.\",\n      \"example\": \"session-abc123\"\n    },\n    \"persistChanges\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether changes are persisted.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advanced-excel/refs/heads/main/json-schema/excel-api-session-schema.json
tags:
- Automation
- Business Intelligence
- Data Analysis
- Data Processing
- Excel
- Microsoft
- Spreadsheets
title: Session
---
