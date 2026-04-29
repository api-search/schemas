---
description: A Snowflake procedure
layout: schema
name: Procedure
properties_list:
- description: Name of the procedure
  name: name
  type: string
- description: What permissions should the procedure execution be called with
  name: execute_as
  type: string
- description: Specifies whether the function/procedure is secure or not
  name: is_secure
  type: boolean
- description: List of arguments for the function/procedure
  name: arguments
  type: array
- description: Specifies a comment for the function/procedure
  name: comment
  type: string
- description: Function/procedure definition
  name: body
  type: string
- description: The date and time when the function/procedure was created
  name: created_on
  type: string
- description: The name of the schema in which the function/procedure exists.
  name: schema_name
  type: string
- description: The name of the database in which the function/procedure exists.
  name: database_name
  type: string
- description: The minimum number of arguments
  name: min_num_arguments
  type: integer
- description: The maximum number of arguments
  name: max_num_arguments
  type: integer
- description: Role that owns the function/procedure
  name: owner
  type: string
- description: The type of role that owns the function/procedure
  name: owner_role_type
  type: string
- description: If the function/procedure is built-in or not (user-defined)
  name: is_builtin
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/procedure-procedure-schema.json
slug: procedure-procedure
source_filename: procedure-procedure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Procedure\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake procedure\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the procedure\"\n    },\n    \"execute_as\": {\n      \"type\": \"string\",\n      \"description\": \"What permissions should the procedure execution be called with\"\n    },\n    \"is_secure\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the function/procedure is secure or not\"\n    },\n    \"arguments\": {\n      \"type\": \"array\",\n      \"description\": \"List of arguments for the function/procedure\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies a comment for the function/procedure\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Function/procedure definition\"\n    },\n    \"created_on\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The date and time when the function/procedure was created\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the schema in which the function/procedure exists.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database in which the function/procedure exists.\"\n    },\n    \"min_num_arguments\": {\n      \"type\": \"integer\",\n      \"description\": \"The minimum number of arguments\"\n    },\n    \"max_num_arguments\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of arguments\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the function/procedure\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the function/procedure\"\n    },\n    \"is_builtin\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"If the function/procedure is built-in or not (user-defined)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/procedure-procedure-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Procedure
---
