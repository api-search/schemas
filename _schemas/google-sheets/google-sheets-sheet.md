---
description: A sheet in a spreadsheet.
layout: schema
name: Sheet
properties_list:
- description: Data in the grid, if this is a grid sheet.
  name: data
  type: array
- description: The ranges that are merged together.
  name: merges
  type: array
- description: The conditional format rules in this sheet.
  name: conditionalFormats
  type: array
- description: The filter views in this sheet.
  name: filterViews
  type: array
- description: The protected ranges in this sheet.
  name: protectedRanges
  type: array
- description: The specifications of every chart on this sheet.
  name: charts
  type: array
- description: The banded (alternating colors) ranges on this sheet.
  name: bandedRanges
  type: array
- description: The slicers on this sheet.
  name: slicers
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-sheet-schema.json
slug: google-sheets-sheet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Sheet\",\n  \"type\": \"object\",\n  \"description\": \"A sheet in a spreadsheet.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Data in the grid, if this is a grid sheet.\"\n    },\n    \"merges\": {\n      \"type\": \"array\",\n      \"description\": \"The ranges that are merged together.\"\n    },\n    \"conditionalFormats\": {\n      \"type\": \"array\",\n      \"description\": \"The conditional format rules in this sheet.\"\n    },\n    \"filterViews\": {\n      \"type\": \"array\",\n      \"description\": \"The filter views in this sheet.\"\n    },\n    \"protectedRanges\": {\n      \"type\": \"array\",\n      \"description\": \"The protected ranges in this sheet.\"\n    },\n    \"charts\": {\n      \"type\": \"array\",\n      \"description\": \"The specifications of every chart on this sheet.\"\n    },\n    \"bandedRanges\": {\n      \"\
  type\": \"array\",\n      \"description\": \"The banded (alternating colors) ranges on this sheet.\"\n    },\n    \"slicers\": {\n      \"type\": \"array\",\n      \"description\": \"The slicers on this sheet.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-sheet-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: Sheet
---
