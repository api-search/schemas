---
description: A bind variable value with its Snowflake data type.
layout: schema
name: BindVariable
properties_list:
- description: The Snowflake data type of the bind variable (e.g. FIXED, TEXT, BOOLEAN, DATE, TIMESTAMP_LTZ, TIMESTAMP_NTZ, TIMESTAMP_TZ).
  name: type
  type: string
- description: The value of the bind variable as a string.
  name: value
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-bind-variable-schema.json
slug: snowflake-sql-rest-bind-variable
source_filename: snowflake-sql-rest-bind-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BindVariable\",\n  \"type\": \"object\",\n  \"description\": \"A bind variable value with its Snowflake data type.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The Snowflake data type of the bind variable (e.g. FIXED, TEXT, BOOLEAN, DATE, TIMESTAMP_LTZ, TIMESTAMP_NTZ, TIMESTAMP_TZ).\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the bind variable as a string.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-bind-variable-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: BindVariable
---
