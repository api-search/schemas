---
description: Represents a color in the RGBA color space. Values are in the range [0, 1].
layout: schema
name: Color
properties_list:
- description: The amount of red in the color as a value in the range [0, 1].
  name: red
  type: number
- description: The amount of green in the color as a value in the range [0, 1].
  name: green
  type: number
- description: The amount of blue in the color as a value in the range [0, 1].
  name: blue
  type: number
- description: The fraction of this color that should be applied to the pixel. A value of 1.0 corresponds to a solid color.
  name: alpha
  type: number
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-color-schema.json
slug: google-sheets-color
source_filename: google-sheets-color-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Color\",\n  \"type\": \"object\",\n  \"description\": \"Represents a color in the RGBA color space. Values are in the range [0, 1].\",\n  \"properties\": {\n    \"red\": {\n      \"type\": \"number\",\n      \"description\": \"The amount of red in the color as a value in the range [0, 1].\"\n    },\n    \"green\": {\n      \"type\": \"number\",\n      \"description\": \"The amount of green in the color as a value in the range [0, 1].\"\n    },\n    \"blue\": {\n      \"type\": \"number\",\n      \"description\": \"The amount of blue in the color as a value in the range [0, 1].\"\n    },\n    \"alpha\": {\n      \"type\": \"number\",\n      \"description\": \"The fraction of this color that should be applied to the pixel. A value of 1.0 corresponds to a solid color.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-color-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: Color
---
