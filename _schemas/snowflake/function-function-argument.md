---
description: An argument of function
layout: schema
name: FunctionArgument
properties_list:
- description: Argument's name
  name: name
  type: string
- description: Argument's type
  name: datatype
  type: string
- description: Argument's value
  name: value
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/function-function-argument-schema.json
slug: function-function-argument
source_filename: function-function-argument-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FunctionArgument\",\n  \"type\": \"object\",\n  \"description\": \"An argument of function\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Argument's name\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"Argument's type\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Argument's value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/function-function-argument-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: FunctionArgument
---
