---
description: ''
layout: schema
name: ScalaFunction
properties_list:
- description: Specifies where Snowflake should write the compiled code for inline function/procedures
  name: target_path
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/procedure-scala-function-schema.json
slug: procedure-scala-function
source_filename: procedure-scala-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScalaFunction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"target_path\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies where Snowflake should write the compiled code for inline function/procedures\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/procedure-scala-function-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ScalaFunction
---
