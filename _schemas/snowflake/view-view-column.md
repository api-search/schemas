---
description: A column specifier in the view
layout: schema
name: ViewColumn
properties_list:
- description: Column name
  name: name
  type: string
- description: Specifies a comment for the column
  name: comment
  type: string
- description: The data type for the column
  name: datatype
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/view-view-column-schema.json
slug: view-view-column
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ViewColumn\",\n  \"type\": \"object\",\n  \"description\": \"A column specifier in the view\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Column name\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the column\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"The data type for the column\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/view-view-column-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ViewColumn
---
