---
description: Data within a range of the spreadsheet.
layout: schema
name: ValueRange
properties_list:
- description: The range the values cover, in A1 notation. For output, this range indicates the entire requested range, even though the values response will include only the non-empty rows and columns.
  name: range
  type: string
- description: The data that was read or to be written. This is an array of arrays, the outer array representing all the data and each inner array representing a major dimension.
  name: values
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-value-range-schema.json
slug: google-sheets-value-range
source_filename: google-sheets-value-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValueRange\",\n  \"type\": \"object\",\n  \"description\": \"Data within a range of the spreadsheet.\",\n  \"properties\": {\n    \"range\": {\n      \"type\": \"string\",\n      \"description\": \"The range the values cover, in A1 notation. For output, this range indicates the entire requested range, even though the values response will include only the non-empty rows and columns.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The data that was read or to be written. This is an array of arrays, the outer array representing all the data and each inner array representing a major dimension.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-value-range-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: ValueRange
---
