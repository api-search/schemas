---
description: An Airtable record representing a single row in a table. Records are the fundamental data units in Airtable, containing field values that correspond to the table's column definitions.
layout: schema
name: Airtable Record
properties_list:
- description: The unique identifier for the record. Record IDs always start with the 'rec' prefix.
  name: id
  type: string
- description: The date and time when the record was created, in ISO 8601 format.
  name: createdTime
  type: string
- description: A mapping of field names (or field IDs when returnFieldsByFieldId is enabled) to their cell values. The keys and value types depend on the table's schema definition.
  name: fields
  type: object
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-record-schema.json
slug: airtable-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/record.json\",\n  \"title\": \"Airtable Record\",\n  \"description\": \"An Airtable record representing a single row in a table. Records are the fundamental data units in Airtable, containing field values that correspond to the table's column definitions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the record. Record IDs always start with the 'rec' prefix.\",\n      \"pattern\": \"^rec[a-zA-Z0-9]+$\",\n      \"examples\": [\"recABC123def456\"]\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the record was created, in ISO 8601 format.\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping of field names (or field IDs when returnFieldsByFieldId\
  \ is enabled) to their cell values. The keys and value types depend on the table's schema definition.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"id\", \"createdTime\", \"fields\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-record-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Record
---
