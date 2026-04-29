---
description: A column in the snowflake catalog iceberg table
layout: schema
name: IcebergTableColumn
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
- description: Argument null return acceptance criteria
  name: nullable
  type: boolean
- description: Default value for the column
  name: default_value
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/iceberg-table-iceberg-table-column-schema.json
slug: iceberg-table-iceberg-table-column
source_filename: iceberg-table-iceberg-table-column-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IcebergTableColumn\",\n  \"type\": \"object\",\n  \"description\": \"A column in the snowflake catalog iceberg table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Column name\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"The data type for the column\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the column\"\n    },\n    \"nullable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Argument null return acceptance criteria\"\n    },\n    \"default_value\": {\n      \"type\": \"string\",\n      \"description\": \"Default value for the column\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/iceberg-table-iceberg-table-column-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: IcebergTableColumn
---
