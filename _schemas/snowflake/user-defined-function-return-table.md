---
description: ''
layout: schema
name: ReturnTable
properties_list:
- description: List of table columns to return
  name: column_list
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/user-defined-function-return-table-schema.json
slug: user-defined-function-return-table
source_filename: user-defined-function-return-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReturnTable\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"column_list\": {\n      \"type\": \"array\",\n      \"description\": \"List of table columns to return\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/user-defined-function-return-table-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ReturnTable
---
