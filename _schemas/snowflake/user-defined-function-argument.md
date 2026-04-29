---
description: ''
layout: schema
name: Argument
properties_list:
- description: Argument name
  name: name
  type: string
- description: Argument data type
  name: datatype
  type: string
- description: Default value of the argument
  name: default_value
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/user-defined-function-argument-schema.json
slug: user-defined-function-argument
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Argument\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Argument name\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"Argument data type\"\n    },\n    \"default_value\": {\n      \"type\": \"string\",\n      \"description\": \"Default value of the argument\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/user-defined-function-argument-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Argument
---
