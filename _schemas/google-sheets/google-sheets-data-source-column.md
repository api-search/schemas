---
description: A column in a data source.
layout: schema
name: DataSourceColumn
properties_list:
- description: The formula of the calculated column.
  name: formula
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-source-column-schema.json
slug: google-sheets-data-source-column
source_filename: google-sheets-data-source-column-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceColumn\",\n  \"type\": \"object\",\n  \"description\": \"A column in a data source.\",\n  \"properties\": {\n    \"formula\": {\n      \"type\": \"string\",\n      \"description\": \"The formula of the calculated column.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-source-column-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataSourceColumn
---
