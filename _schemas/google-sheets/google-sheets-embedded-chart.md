---
description: A chart embedded in a sheet.
layout: schema
name: EmbeddedChart
properties_list:
- description: The ID of the chart.
  name: chartId
  type: integer
- description: The specification of the chart.
  name: spec
  type: object
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-embedded-chart-schema.json
slug: google-sheets-embedded-chart
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmbeddedChart\",\n  \"type\": \"object\",\n  \"description\": \"A chart embedded in a sheet.\",\n  \"properties\": {\n    \"chartId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the chart.\"\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"The specification of the chart.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-embedded-chart-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: EmbeddedChart
---
