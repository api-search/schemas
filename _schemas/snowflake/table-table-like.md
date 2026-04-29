---
description: Create table like an existing table
layout: schema
name: TableLike
properties_list:
- description: Specifies the name for the table, must be unique for the schema in which the table is created
  name: name
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/table-table-like-schema.json
slug: table-table-like
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableLike\",\n  \"type\": \"object\",\n  \"description\": \"Create table like an existing table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name for the table, must be unique for the schema in which the table is created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/table-table-like-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TableLike
---
