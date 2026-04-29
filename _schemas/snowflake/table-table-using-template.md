---
description: Create table using template
layout: schema
name: TableUsingTemplate
properties_list:
- description: Specifies the name for the table, must be unique for the schema in which the table is created
  name: name
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/table-table-using-template-schema.json
slug: table-table-using-template
source_filename: table-table-using-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableUsingTemplate\",\n  \"type\": \"object\",\n  \"description\": \"Create table using template\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name for the table, must be unique for the schema in which the table is created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/table-table-using-template-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TableUsingTemplate
---
