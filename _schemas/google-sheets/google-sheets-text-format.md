---
description: The format of a run of text in a cell.
layout: schema
name: TextFormat
properties_list:
- description: The font family.
  name: fontFamily
  type: string
- description: The size of the font.
  name: fontSize
  type: integer
- description: True if the text is bold.
  name: bold
  type: boolean
- description: True if the text is italicized.
  name: italic
  type: boolean
- description: True if the text has a strikethrough.
  name: strikethrough
  type: boolean
- description: True if the text is underlined.
  name: underline
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-text-format-schema.json
slug: google-sheets-text-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextFormat\",\n  \"type\": \"object\",\n  \"description\": \"The format of a run of text in a cell.\",\n  \"properties\": {\n    \"fontFamily\": {\n      \"type\": \"string\",\n      \"description\": \"The font family.\"\n    },\n    \"fontSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the font.\"\n    },\n    \"bold\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the text is bold.\"\n    },\n    \"italic\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the text is italicized.\"\n    },\n    \"strikethrough\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the text has a strikethrough.\"\n    },\n    \"underline\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the text is underlined.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-text-format-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: TextFormat
---
