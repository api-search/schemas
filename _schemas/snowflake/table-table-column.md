---
description: A column in the table
layout: schema
name: TableColumn
properties_list:
- description: Column name
  name: name
  type: string
- description: The data type for the column
  name: datatype
  type: string
- description: Specifies that the column does allow NULL values or not.
  name: nullable
  type: boolean
- description: Specifies the collation to use for column operations such as string comparison
  name: collate
  type: string
- description: Specifies whether a default value is automatically inserted in the column if a value is not explicitly specified via an INSERT or CREATE TABLE AS SELECT statement
  name: default
  type: string
- description: ''
  name: autoincrement
  type: boolean
- description: The default value for the column starts with the specified number
  name: autoincrement_start
  type: integer
- description: Each successive value for the column automatically increments by the specified amount
  name: autoincrement_increment
  type: integer
- description: ''
  name: constraints
  type: array
- description: Specifies a comment for the column
  name: comment
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/table-table-column-schema.json
slug: table-table-column
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableColumn\",\n  \"type\": \"object\",\n  \"description\": \"A column in the table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Column name\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"The data type for the column\"\n    },\n    \"nullable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies that the column does allow NULL values or not.\"\n    },\n    \"collate\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the collation to use for column operations such as string comparison\"\n    },\n    \"default\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether a default value is automatically inserted in the column if a value is not explicitly specified via an INSERT or CREATE TABLE AS SELECT statement\"\n    },\n    \"autoincrement\": {\n   \
  \   \"type\": \"boolean\"\n    },\n    \"autoincrement_start\": {\n      \"type\": \"integer\",\n      \"description\": \"The default value for the column starts with the specified number\"\n    },\n    \"autoincrement_increment\": {\n      \"type\": \"integer\",\n      \"description\": \"Each successive value for the column automatically increments by the specified amount\"\n    },\n    \"constraints\": {\n      \"type\": \"array\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the column\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/table-table-column-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TableColumn
---
