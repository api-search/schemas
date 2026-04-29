---
description: An Airtable table is a collection of records organized with a defined set of fields and views within a base. Tables define the structure and schema of the data they contain.
layout: schema
name: Airtable Table
properties_list:
- description: The unique identifier for the table. Table IDs always start with the 'tbl' prefix.
  name: id
  type: string
- description: The display name of the table.
  name: name
  type: string
- description: An optional description of the table's purpose and contents.
  name: description
  type:
  - string
  - 'null'
- description: The ID of the primary field for this table. The primary field serves as the main identifier for records.
  name: primaryFieldId
  type: string
- description: The field definitions (columns) in the table.
  name: fields
  type: array
- description: The view definitions in the table.
  name: views
  type: array
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-table-schema.json
slug: airtable-table
source_filename: airtable-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/table.json\",\n  \"title\": \"Airtable Table\",\n  \"description\": \"An Airtable table is a collection of records organized with a defined set of fields and views within a base. Tables define the structure and schema of the data they contain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the table. Table IDs always start with the 'tbl' prefix.\",\n      \"pattern\": \"^tbl[a-zA-Z0-9]+$\",\n      \"examples\": [\"tblABC123def456\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the table.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional description of the table's purpose and contents.\"\n    },\n    \"primaryFieldId\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"The ID of the primary field for this table. The primary field serves as the main identifier for records.\",\n      \"pattern\": \"^fld[a-zA-Z0-9]+$\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"The field definitions (columns) in the table.\",\n      \"items\": {\n        \"$ref\": \"https://schemas.airtable.com/field.json\"\n      }\n    },\n    \"views\": {\n      \"type\": \"array\",\n      \"description\": \"The view definitions in the table.\",\n      \"items\": {\n        \"$ref\": \"https://schemas.airtable.com/view.json\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"fields\", \"views\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-table-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Table
---
