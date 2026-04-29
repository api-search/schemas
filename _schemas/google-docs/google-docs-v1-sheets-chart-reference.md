---
description: A reference to a linked chart embedded from Google Sheets.
layout: schema
name: SheetsChartReference
properties_list:
- description: The ID of the Google Sheets spreadsheet that contains the source chart.
  name: spreadsheetId
  type: string
- description: The ID of the specific chart in the Sheets spreadsheet.
  name: chartId
  type: integer
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-sheets-chart-reference-schema.json
slug: google-docs-v1-sheets-chart-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SheetsChartReference\",\n  \"type\": \"object\",\n  \"description\": \"A reference to a linked chart embedded from Google Sheets.\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Google Sheets spreadsheet that contains the source chart.\"\n    },\n    \"chartId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the specific chart in the Sheets spreadsheet.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-sheets-chart-reference-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: SheetsChartReference
---
