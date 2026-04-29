---
description: ''
layout: schema
name: ReturnDataType
properties_list:
- description: Return data type
  name: datatype
  type: string
- description: Argument null return acceptance criteria
  name: nullable
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/user-defined-function-return-data-type-schema.json
slug: user-defined-function-return-data-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReturnDataType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"Return data type\"\n    },\n    \"nullable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Argument null return acceptance criteria\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/user-defined-function-return-data-type-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ReturnDataType
---
