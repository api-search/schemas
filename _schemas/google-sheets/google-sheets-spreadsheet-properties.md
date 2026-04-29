---
description: Properties of a spreadsheet.
layout: schema
name: SpreadsheetProperties
properties_list:
- description: The title of the spreadsheet.
  name: title
  type: string
- description: 'The locale of the spreadsheet in one of the following formats: an ISO 639-1 language code, an ISO 639-2 language code, or a combination of the ISO language code and country code (e.g. en, eng, en_US).'
  name: locale
  type: string
- description: The amount of time to wait before volatile functions are recalculated.
  name: autoRecalc
  type: string
- description: The time zone of the spreadsheet in CLDR format (e.g. America/New_York).
  name: timeZone
  type: string
- description: Whether to allow external URL access for image and import functions.
  name: importFunctionsExternalUrlAccessAllowed
  type: boolean
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-spreadsheet-properties-schema.json
slug: google-sheets-spreadsheet-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SpreadsheetProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of a spreadsheet.\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the spreadsheet.\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"The locale of the spreadsheet in one of the following formats: an ISO 639-1 language code, an ISO 639-2 language code, or a combination of the ISO language code and country code (e.g. en, eng, en_US).\"\n    },\n    \"autoRecalc\": {\n      \"type\": \"string\",\n      \"description\": \"The amount of time to wait before volatile functions are recalculated.\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone of the spreadsheet in CLDR format (e.g. America/New_York).\"\n    },\n    \"importFunctionsExternalUrlAccessAllowed\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether to allow external URL access for image and import functions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-spreadsheet-properties-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: SpreadsheetProperties
---
