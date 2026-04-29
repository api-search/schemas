---
description: The format of a cell.
layout: schema
name: CellFormat
properties_list:
- description: The horizontal alignment of the value in the cell.
  name: horizontalAlignment
  type: string
- description: The vertical alignment of the value in the cell.
  name: verticalAlignment
  type: string
- description: The wrap strategy for the value in the cell.
  name: wrapStrategy
  type: string
- description: The direction of the text in the cell.
  name: textDirection
  type: string
- description: How a hyperlink, if any, should be displayed in the cell.
  name: hyperlinkDisplayType
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-cell-format-schema.json
slug: google-sheets-cell-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CellFormat\",\n  \"type\": \"object\",\n  \"description\": \"The format of a cell.\",\n  \"properties\": {\n    \"horizontalAlignment\": {\n      \"type\": \"string\",\n      \"description\": \"The horizontal alignment of the value in the cell.\"\n    },\n    \"verticalAlignment\": {\n      \"type\": \"string\",\n      \"description\": \"The vertical alignment of the value in the cell.\"\n    },\n    \"wrapStrategy\": {\n      \"type\": \"string\",\n      \"description\": \"The wrap strategy for the value in the cell.\"\n    },\n    \"textDirection\": {\n      \"type\": \"string\",\n      \"description\": \"The direction of the text in the cell.\"\n    },\n    \"hyperlinkDisplayType\": {\n      \"type\": \"string\",\n      \"description\": \"How a hyperlink, if any, should be displayed in the cell.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-cell-format-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: CellFormat
---
