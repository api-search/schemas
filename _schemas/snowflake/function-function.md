---
description: A Snowflake function
layout: schema
name: Function
properties_list:
- description: ''
  name: function_type
  type: string
- description: Specifies the name for the function, must be unique for the schema in which the function is created
  name: name
  type: string
- description: ''
  name: arguments
  type: array
- description: Specifies the type for the function return value.
  name: returns
  type: string
- description: Specifies the max rows for batch operation.
  name: max_batch_rows
  type: integer
- description: Date and time when the function was created.
  name: created_on
  type: string
- description: Function's arguments.
  name: signature
  type: string
- description: Function's language.
  name: language
  type: string
- description: Function's body.
  name: body
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/function-function-schema.json
slug: function-function
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Function\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake function\",\n  \"properties\": {\n    \"function_type\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the name for the function, must be unique for the schema in which the function is created\"\n    },\n    \"arguments\": {\n      \"type\": \"array\"\n    },\n    \"returns\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the type for the function return value.\"\n    },\n    \"max_batch_rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Specifies the max rows for batch operation.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the function was created.\"\n    },\n    \"signature\": {\n      \"type\": \"string\",\n      \"description\": \"Function's arguments.\"\
  \n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Function's language.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Function's body.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/function-function-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Function
---
