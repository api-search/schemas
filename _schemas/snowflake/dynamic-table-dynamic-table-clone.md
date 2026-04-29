---
description: Clone dynamic table
layout: schema
name: DynamicTableClone
properties_list:
- description: Specifies the name for the dynamic table, must be unique for the schema in which the dynamic table is created
  name: name
  type: string
- description: Specifies the name of the warehouse that provides the compute resources for refreshing the dynamic table
  name: warehouse
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/dynamic-table-dynamic-table-clone-schema.json
slug: dynamic-table-dynamic-table-clone
source_filename: dynamic-table-dynamic-table-clone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DynamicTableClone\",\n  \"type\": \"object\",\n  \"description\": \"Clone dynamic table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name for the dynamic table, must be unique for the schema in which the dynamic table is created\"\n    },\n    \"warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name of the warehouse that provides the compute resources for refreshing the dynamic table\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/dynamic-table-dynamic-table-clone-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: DynamicTableClone
---
