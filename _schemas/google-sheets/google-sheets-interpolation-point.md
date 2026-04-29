---
description: A single interpolation point on a gradient conditional format.
layout: schema
name: InterpolationPoint
properties_list:
- description: How the value should be interpreted.
  name: type
  type: string
- description: The value this interpolation point uses.
  name: value
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-interpolation-point-schema.json
slug: google-sheets-interpolation-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InterpolationPoint\",\n  \"type\": \"object\",\n  \"description\": \"A single interpolation point on a gradient conditional format.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"How the value should be interpreted.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value this interpolation point uses.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-interpolation-point-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: InterpolationPoint
---
