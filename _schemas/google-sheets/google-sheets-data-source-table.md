---
description: A data source table, which allows the user to import a static table of data from the DataSource into Sheets.
layout: schema
name: DataSourceTable
properties_list:
- description: The ID of the data source the data source table is associated with.
  name: dataSourceId
  type: string
- description: The type to select columns for the data source table.
  name: columnSelectionType
  type: string
- description: Columns selected for the data source table.
  name: columns
  type: array
- description: Filter specifications in the data source table.
  name: filterSpecs
  type: array
- description: Sort specifications in the data source table.
  name: sortSpecs
  type: array
- description: The limit of rows to return.
  name: rowLimit
  type: integer
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-source-table-schema.json
slug: google-sheets-data-source-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceTable\",\n  \"type\": \"object\",\n  \"description\": \"A data source table, which allows the user to import a static table of data from the DataSource into Sheets.\",\n  \"properties\": {\n    \"dataSourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the data source the data source table is associated with.\"\n    },\n    \"columnSelectionType\": {\n      \"type\": \"string\",\n      \"description\": \"The type to select columns for the data source table.\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"Columns selected for the data source table.\"\n    },\n    \"filterSpecs\": {\n      \"type\": \"array\",\n      \"description\": \"Filter specifications in the data source table.\"\n    },\n    \"sortSpecs\": {\n      \"type\": \"array\",\n      \"description\": \"Sort specifications in the data source table.\"\n    },\n\
  \    \"rowLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"The limit of rows to return.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-source-table-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataSourceTable
---
