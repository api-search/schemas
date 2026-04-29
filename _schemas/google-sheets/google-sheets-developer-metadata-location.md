---
description: A location where metadata may be associated in a spreadsheet.
layout: schema
name: DeveloperMetadataLocation
properties_list:
- description: The type of location this object represents.
  name: locationType
  type: string
- description: True when metadata is associated with an entire spreadsheet.
  name: spreadsheet
  type: boolean
- description: The ID of the sheet when metadata is associated with an entire sheet.
  name: sheetId
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-developer-metadata-location-schema.json
slug: google-sheets-developer-metadata-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeveloperMetadataLocation\",\n  \"type\": \"object\",\n  \"description\": \"A location where metadata may be associated in a spreadsheet.\",\n  \"properties\": {\n    \"locationType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of location this object represents.\"\n    },\n    \"spreadsheet\": {\n      \"type\": \"boolean\",\n      \"description\": \"True when metadata is associated with an entire spreadsheet.\"\n    },\n    \"sheetId\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the sheet when metadata is associated with an entire sheet.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-developer-metadata-location-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DeveloperMetadataLocation
---
