---
description: Represents spreadsheet theme.
layout: schema
name: SpreadsheetTheme
properties_list:
- description: Name of the primary font family.
  name: primaryFontFamily
  type: string
- description: The spreadsheet theme color pairs.
  name: themeColors
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-spreadsheet-theme-schema.json
slug: google-sheets-spreadsheet-theme
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpreadsheetTheme\",\n  \"type\": \"object\",\n  \"description\": \"Represents spreadsheet theme.\",\n  \"properties\": {\n    \"primaryFontFamily\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the primary font family.\"\n    },\n    \"themeColors\": {\n      \"type\": \"array\",\n      \"description\": \"The spreadsheet theme color pairs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-spreadsheet-theme-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: SpreadsheetTheme
---
