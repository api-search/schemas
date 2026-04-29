---
description: A border along a cell.
layout: schema
name: Border
properties_list:
- description: The style of the border.
  name: style
  type: string
- description: The width of the border, in pixels. Deprecated; the width is determined by the style.
  name: width
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-border-schema.json
slug: google-sheets-border
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Border\",\n  \"type\": \"object\",\n  \"description\": \"A border along a cell.\",\n  \"properties\": {\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"The style of the border.\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"The width of the border, in pixels. Deprecated; the width is determined by the style.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-border-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: Border
---
