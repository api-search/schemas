---
description: ''
layout: schema
name: FunctionLanguage
properties_list:
- description: 'Language that the function/procedure is written in. Possible values include: JAVA, JAVASCRIPT, PYTHON, SCALA, SQL'
  name: language
  type: string
- description: Decide if the function/procedure can receive null input
  name: called_on_null_input
  type: boolean
- description: 'Specifies the behavior of the UDF when returning results. This Field is deprecated for Procedure. If true, UDF might return different values for different rows, even for the same input. This field is '
  name: is_volatile
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/user-defined-function-function-language-schema.json
slug: user-defined-function-function-language
source_filename: user-defined-function-function-language-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FunctionLanguage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language that the function/procedure is written in. Possible values include: JAVA, JAVASCRIPT, PYTHON, SCALA, SQL\"\n    },\n    \"called_on_null_input\": {\n      \"type\": \"boolean\",\n      \"description\": \"Decide if the function/procedure can receive null input\"\n    },\n    \"is_volatile\": {\n      \"type\": \"boolean\",\n      \"description\": \" Specifies the behavior of the UDF when returning results. This Field is deprecated for Procedure.\\n            \\n            If true, UDF might return different values for different rows, even for the same input. \\n            This field is deprecated for Procedure.\\n\\n            If false, UDF assumes that the function, when called with the same inputs, will always return the same result. \\n\
  \            This guarantee is not checked. Specifying IMMUTABLE for a UDF that returns different values for the same input will result in undefined behavior.\\n        \"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/user-defined-function-function-language-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: FunctionLanguage
---
