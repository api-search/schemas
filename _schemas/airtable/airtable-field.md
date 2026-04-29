---
description: An Airtable field represents a column in a table, defining the data type, validation rules, and display configuration for values stored in that column.
layout: schema
name: Airtable Field
properties_list:
- description: The unique identifier for the field. Field IDs always start with the 'fld' prefix.
  name: id
  type: string
- description: The display name of the field.
  name: name
  type: string
- description: The data type of the field, which determines what values can be stored and how they are displayed.
  name: type
  type: string
- description: An optional description of the field.
  name: description
  type:
  - string
  - 'null'
- description: Configuration options specific to the field type. For example, singleSelect fields have a choices array, number fields have a precision setting, and linked record fields specify the linked table.
  name: options
  type: object
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-field-schema.json
slug: airtable-field
source_filename: airtable-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/field.json\",\n  \"title\": \"Airtable Field\",\n  \"description\": \"An Airtable field represents a column in a table, defining the data type, validation rules, and display configuration for values stored in that column.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the field. Field IDs always start with the 'fld' prefix.\",\n      \"pattern\": \"^fld[a-zA-Z0-9]+$\",\n      \"examples\": [\"fldABC123def456\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the field.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the field, which determines what values can be stored and how they are displayed.\",\n      \"enum\": [\n        \"singleLineText\",\n        \"email\",\n\
  \        \"url\",\n        \"multilineText\",\n        \"number\",\n        \"percent\",\n        \"currency\",\n        \"singleSelect\",\n        \"multipleSelects\",\n        \"singleCollaborator\",\n        \"multipleCollaborators\",\n        \"multipleRecordLinks\",\n        \"date\",\n        \"dateTime\",\n        \"phoneNumber\",\n        \"multipleAttachments\",\n        \"checkbox\",\n        \"formula\",\n        \"createdTime\",\n        \"rollup\",\n        \"count\",\n        \"lookup\",\n        \"multipleLookupValues\",\n        \"autoNumber\",\n        \"barcode\",\n        \"rating\",\n        \"richText\",\n        \"duration\",\n        \"lastModifiedTime\",\n        \"button\",\n        \"createdBy\",\n        \"lastModifiedBy\",\n        \"externalSyncSource\",\n        \"aiText\"\n      ]\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional description of the field.\"\n    },\n    \"options\": {\n      \"\
  type\": \"object\",\n      \"description\": \"Configuration options specific to the field type. For example, singleSelect fields have a choices array, number fields have a precision setting, and linked record fields specify the linked table.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-field-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Field
---
