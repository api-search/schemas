---
description: An import operation
layout: schema
name: Import
properties_list:
- description: The unique identifier of the import
  name: id
  type: string
- description: The display name of the import
  name: name
  type: string
- description: The state of the import
  name: importState
  type: string
- description: When the import was created
  name: createdDateTime
  type: string
- description: When the import was last updated
  name: updatedDateTime
  type: string
- description: Reports created by this import
  name: reports
  type: array
- description: Datasets created by this import
  name: datasets
  type: array
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-import-schema.json
slug: power-bi-rest-import
source_filename: power-bi-rest-import-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Import\",\n  \"type\": \"object\",\n  \"description\": \"An import operation\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the import\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the import\"\n    },\n    \"importState\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the import\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the import was created\"\n    },\n    \"updatedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the import was last updated\"\n    },\n    \"reports\": {\n      \"type\": \"array\",\n      \"description\": \"Reports created by this import\"\n    },\n    \"datasets\": {\n      \"type\": \"array\",\n      \"description\": \"Datasets created by this\
  \ import\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-import-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Import
---
