---
description: Foreign keys link data in one table to the data in another table.
layout: schema
name: ForeignKey
properties_list:
- description: ''
  name: referenced_table_name
  type: string
- description: ''
  name: referenced_column_names
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/table-foreign-key-schema.json
slug: table-foreign-key
source_filename: table-foreign-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ForeignKey\",\n  \"type\": \"object\",\n  \"description\": \"Foreign keys link data in one table to the data in another table.\",\n  \"properties\": {\n    \"referenced_table_name\": {\n      \"type\": \"string\"\n    },\n    \"referenced_column_names\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/table-foreign-key-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ForeignKey
---
