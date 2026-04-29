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
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/procedure-function-language-schema.json
slug: procedure-function-language
source_filename: procedure-function-language-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FunctionLanguage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language that the function/procedure is written in. Possible values include: JAVA, JAVASCRIPT, PYTHON, SCALA, SQL\"\n    },\n    \"called_on_null_input\": {\n      \"type\": \"boolean\",\n      \"description\": \"Decide if the function/procedure can receive null input\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/procedure-function-language-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: FunctionLanguage
---
