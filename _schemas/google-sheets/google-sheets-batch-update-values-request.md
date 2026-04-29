---
description: The request for updating more than one range of values in a spreadsheet.
layout: schema
name: BatchUpdateValuesRequest
properties_list:
- description: The new values to apply to the spreadsheet.
  name: data
  type: array
- description: Determines if the update response should include the values of the cells that were updated.
  name: includeValuesInResponse
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-batch-update-values-request-schema.json
slug: google-sheets-batch-update-values-request
source_filename: google-sheets-batch-update-values-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchUpdateValuesRequest\",\n  \"type\": \"object\",\n  \"description\": \"The request for updating more than one range of values in a spreadsheet.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The new values to apply to the spreadsheet.\"\n    },\n    \"includeValuesInResponse\": {\n      \"type\": \"boolean\",\n      \"description\": \"Determines if the update response should include the values of the cells that were updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-batch-update-values-request-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BatchUpdateValuesRequest
---
