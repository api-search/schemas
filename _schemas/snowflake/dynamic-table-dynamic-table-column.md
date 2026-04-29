---
description: A column in the dynamic table
layout: schema
name: DynamicTableColumn
properties_list:
- description: Column name
  name: name
  type: string
- description: The data type for the column
  name: datatype
  type: string
- description: Specifies a comment for the column
  name: comment
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/dynamic-table-dynamic-table-column-schema.json
slug: dynamic-table-dynamic-table-column
source_filename: dynamic-table-dynamic-table-column-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DynamicTableColumn\",\n  \"type\": \"object\",\n  \"description\": \"A column in the dynamic table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Column name\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"The data type for the column\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the column\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/dynamic-table-dynamic-table-column-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: DynamicTableColumn
---
