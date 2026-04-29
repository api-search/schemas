---
description: ''
layout: schema
name: ColumnType
properties_list:
- description: Argument name
  name: name
  type: string
- description: Argument data type
  name: datatype
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/user-defined-function-column-type-schema.json
slug: user-defined-function-column-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColumnType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Argument name\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"Argument data type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/user-defined-function-column-type-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ColumnType
---
