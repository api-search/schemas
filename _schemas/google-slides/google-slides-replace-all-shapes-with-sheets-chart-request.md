---
description: Replaces all shapes that match the given criteria with the provided Google Sheets chart.
layout: schema
name: ReplaceAllShapesWithSheetsChartRequest
properties_list:
- description: The ID of the Google Sheets spreadsheet.
  name: spreadsheetId
  type: string
- description: The ID of the specific chart in the Google Sheets spreadsheet.
  name: chartId
  type: integer
- description: The mode with which the chart is linked to the source spreadsheet.
  name: linkingMode
  type: string
- description: If non-empty, limits to the given pages.
  name: pageObjectIds
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-replace-all-shapes-with-sheets-chart-request-schema.json
slug: google-slides-replace-all-shapes-with-sheets-chart-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReplaceAllShapesWithSheetsChartRequest\",\n  \"type\": \"object\",\n  \"description\": \"Replaces all shapes that match the given criteria with the provided Google Sheets chart.\\n\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Google Sheets spreadsheet.\"\n    },\n    \"chartId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the specific chart in the Google Sheets spreadsheet.\"\n    },\n    \"linkingMode\": {\n      \"type\": \"string\",\n      \"description\": \"The mode with which the chart is linked to the source spreadsheet.\"\n    },\n    \"pageObjectIds\": {\n      \"type\": \"array\",\n      \"description\": \"If non-empty, limits to the given pages.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-replace-all-shapes-with-sheets-chart-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: ReplaceAllShapesWithSheetsChartRequest
---
