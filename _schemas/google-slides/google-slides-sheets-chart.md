---
description: A PageElement kind representing a linked chart embedded from Google Sheets.
layout: schema
name: SheetsChart
properties_list:
- description: The ID of the Google Sheets spreadsheet that contains the source chart.
  name: spreadsheetId
  type: string
- description: The ID of the specific chart in the Google Sheets spreadsheet.
  name: chartId
  type: integer
- description: The URL of an image of the embedded chart, with a default lifetime of 30 minutes.
  name: contentUrl
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-sheets-chart-schema.json
slug: google-slides-sheets-chart
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SheetsChart\",\n  \"type\": \"object\",\n  \"description\": \"A PageElement kind representing a linked chart embedded from Google Sheets.\\n\",\n  \"properties\": {\n    \"spreadsheetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Google Sheets spreadsheet that contains the source chart.\"\n    },\n    \"chartId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the specific chart in the Google Sheets spreadsheet.\"\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of an image of the embedded chart, with a default lifetime of 30 minutes.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-sheets-chart-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: SheetsChart
---
