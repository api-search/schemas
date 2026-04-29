---
description: ''
layout: schema
name: CallArgument
properties_list:
- description: Name of the call argument
  name: name
  type: string
- description: Call argument data type
  name: datatype
  type: string
- description: Value of the call argument
  name: value
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/procedure-call-argument-schema.json
slug: procedure-call-argument
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallArgument\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the call argument\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"Call argument data type\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Value of the call argument\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/procedure-call-argument-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: CallArgument
---
