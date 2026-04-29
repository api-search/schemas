---
description: Creates an embedded Google Sheets chart.
layout: schema
name: CreateSheetsChartRequest
properties_list:
- description: A user-supplied object ID.
  name: objectId
  type: string
- description: The ID of the Google Sheets spreadsheet that contains the chart.
  name: spreadsheetId
  type: string
- description: The ID of the specific chart in the Google Sheets spreadsheet.
  name: chartId
  type: integer
- description: The mode with which the chart is linked to the source spreadsheet.
  name: linkingMode
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-create-sheets-chart-request-schema.json
slug: google-slides-create-sheets-chart-request
source_filename: google-slides-create-sheets-chart-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateSheetsChartRequest\",\n  \"type\": \"object\",\n  \"description\": \"Creates an embedded Google Sheets chart.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied object ID.\"\n    },\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Google Sheets spreadsheet that contains the chart.\"\n    },\n    \"chartId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the specific chart in the Google Sheets spreadsheet.\"\n    },\n    \"linkingMode\": {\n      \"type\": \"string\",\n      \"description\": \"The mode with which the chart is linked to the source spreadsheet.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-create-sheets-chart-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: CreateSheetsChartRequest
---
