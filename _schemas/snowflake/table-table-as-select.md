---
description: Create table as select
layout: schema
name: TableAsSelect
properties_list:
- description: Specifies the name for the table, must be unique for the schema in which the table is created
  name: name
  type: string
- description: ''
  name: columns
  type: array
- description: Specifies one or more columns or column expressions in the table as the clustering key
  name: cluster_by
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/table-table-as-select-schema.json
slug: table-table-as-select
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableAsSelect\",\n  \"type\": \"object\",\n  \"description\": \"Create table as select\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name for the table, must be unique for the schema in which the table is created\"\n    },\n    \"columns\": {\n      \"type\": \"array\"\n    },\n    \"cluster_by\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies one or more columns or column expressions in the table as the clustering key\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/table-table-as-select-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TableAsSelect
---
