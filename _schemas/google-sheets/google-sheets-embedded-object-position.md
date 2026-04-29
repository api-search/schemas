---
description: The position of an embedded object such as a chart.
layout: schema
name: EmbeddedObjectPosition
properties_list:
- description: The sheet this is on.
  name: sheetId
  type: integer
- description: The position at which the object is overlaid on top of a grid.
  name: overlayPosition
  type: object
- description: If true, the embedded object is put on a new sheet whose ID is chosen for you.
  name: newSheet
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-embedded-object-position-schema.json
slug: google-sheets-embedded-object-position
source_filename: google-sheets-embedded-object-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmbeddedObjectPosition\",\n  \"type\": \"object\",\n  \"description\": \"The position of an embedded object such as a chart.\",\n  \"properties\": {\n    \"sheetId\": {\n      \"type\": \"integer\",\n      \"description\": \"The sheet this is on.\"\n    },\n    \"overlayPosition\": {\n      \"type\": \"object\",\n      \"description\": \"The position at which the object is overlaid on top of a grid.\"\n    },\n    \"newSheet\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the embedded object is put on a new sheet whose ID is chosen for you.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-embedded-object-position-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: EmbeddedObjectPosition
---
