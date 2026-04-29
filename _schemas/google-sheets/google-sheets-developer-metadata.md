---
description: Developer metadata associated with a location or object in a spreadsheet.
layout: schema
name: DeveloperMetadata
properties_list:
- description: The spreadsheet-scoped unique ID that identifies the metadata.
  name: metadataId
  type: integer
- description: The metadata key.
  name: metadataKey
  type: string
- description: Data associated with the metadata's key.
  name: metadataValue
  type: string
- description: The metadata visibility.
  name: visibility
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-developer-metadata-schema.json
slug: google-sheets-developer-metadata
source_filename: google-sheets-developer-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeveloperMetadata\",\n  \"type\": \"object\",\n  \"description\": \"Developer metadata associated with a location or object in a spreadsheet.\",\n  \"properties\": {\n    \"metadataId\": {\n      \"type\": \"integer\",\n      \"description\": \"The spreadsheet-scoped unique ID that identifies the metadata.\"\n    },\n    \"metadataKey\": {\n      \"type\": \"string\",\n      \"description\": \"The metadata key.\"\n    },\n    \"metadataValue\": {\n      \"type\": \"string\",\n      \"description\": \"Data associated with the metadata's key.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"The metadata visibility.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-developer-metadata-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DeveloperMetadata
---
