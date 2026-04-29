---
description: A slicer in a sheet.
layout: schema
name: Slicer
properties_list:
- description: The ID of the slicer.
  name: slicerId
  type: integer
- description: The specification of the slicer.
  name: spec
  type: object
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-slicer-schema.json
slug: google-sheets-slicer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Slicer\",\n  \"type\": \"object\",\n  \"description\": \"A slicer in a sheet.\",\n  \"properties\": {\n    \"slicerId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the slicer.\"\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"The specification of the slicer.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-slicer-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: Slicer
---
