---
description: The amount of padding around the cell, in pixels.
layout: schema
name: Padding
properties_list:
- description: The top padding of the cell.
  name: top
  type: integer
- description: The right padding of the cell.
  name: right
  type: integer
- description: The bottom padding of the cell.
  name: bottom
  type: integer
- description: The left padding of the cell.
  name: left
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-padding-schema.json
slug: google-sheets-padding
source_filename: google-sheets-padding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Padding\",\n  \"type\": \"object\",\n  \"description\": \"The amount of padding around the cell, in pixels.\",\n  \"properties\": {\n    \"top\": {\n      \"type\": \"integer\",\n      \"description\": \"The top padding of the cell.\"\n    },\n    \"right\": {\n      \"type\": \"integer\",\n      \"description\": \"The right padding of the cell.\"\n    },\n    \"bottom\": {\n      \"type\": \"integer\",\n      \"description\": \"The bottom padding of the cell.\"\n    },\n    \"left\": {\n      \"type\": \"integer\",\n      \"description\": \"The left padding of the cell.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-padding-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: Padding
---
