---
description: The rotation applied to text in a cell.
layout: schema
name: TextRotation
properties_list:
- description: The angle between the standard orientation and the desired orientation. Measured in degrees. Valid values are between -90 and 90.
  name: angle
  type: integer
- description: If true, text reads top to bottom, but the orientation of individual characters is unchanged.
  name: vertical
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-text-rotation-schema.json
slug: google-sheets-text-rotation
source_filename: google-sheets-text-rotation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextRotation\",\n  \"type\": \"object\",\n  \"description\": \"The rotation applied to text in a cell.\",\n  \"properties\": {\n    \"angle\": {\n      \"type\": \"integer\",\n      \"description\": \"The angle between the standard orientation and the desired orientation. Measured in degrees. Valid values are between -90 and 90.\"\n    },\n    \"vertical\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, text reads top to bottom, but the orientation of individual characters is unchanged.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-text-rotation-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: TextRotation
---
