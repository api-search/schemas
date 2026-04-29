---
description: Describes a column in the result set.
layout: schema
name: ColumnDefinition
properties_list:
- description: Name of the column.
  name: name
  type: string
- description: Snowflake data type of the column (e.g. FIXED, TEXT, BOOLEAN, DATE, TIMESTAMP_NTZ, VARIANT, ARRAY, OBJECT).
  name: type
  type: string
- description: Maximum length of the column data.
  name: length
  type: integer
- description: Precision of numeric data.
  name: precision
  type: integer
- description: Scale of numeric data.
  name: scale
  type: integer
- description: Whether the column allows null values.
  name: nullable
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-column-definition-schema.json
slug: snowflake-sql-rest-column-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColumnDefinition\",\n  \"type\": \"object\",\n  \"description\": \"Describes a column in the result set.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the column.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Snowflake data type of the column (e.g. FIXED, TEXT, BOOLEAN, DATE, TIMESTAMP_NTZ, VARIANT, ARRAY, OBJECT).\"\n    },\n    \"length\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum length of the column data.\"\n    },\n    \"precision\": {\n      \"type\": \"integer\",\n      \"description\": \"Precision of numeric data.\"\n    },\n    \"scale\": {\n      \"type\": \"integer\",\n      \"description\": \"Scale of numeric data.\"\n    },\n    \"nullable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the column allows null values.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-column-definition-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ColumnDefinition
---
