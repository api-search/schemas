---
description: ''
layout: schema
name: ReturnType
properties_list:
- description: Type of the return, can be either DATATYPE or TABLE
  name: type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/procedure-return-type-schema.json
slug: procedure-return-type
source_filename: procedure-return-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReturnType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the return, can be either DATATYPE or TABLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/procedure-return-type-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ReturnType
---
