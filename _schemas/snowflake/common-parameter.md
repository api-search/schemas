---
description: Snowflake parameter defined at the system, account, user, session, or object level.
layout: schema
name: Parameter
properties_list:
- description: Parameter name.
  name: name
  type: string
- description: Parameter value.
  name: value
  type: string
- description: Default parameter value.
  name: defaultValue
  type: string
- description: Data type of the parameter value. Either BOOLEAN, NUMBER, FLOAT, or STRING.
  name: dataType
  type: string
- description: Level at which parameter is defined.
  name: level
  type: string
- description: Parameter description.
  name: description
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-parameter-schema.json
slug: common-parameter
source_filename: common-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parameter\",\n  \"type\": \"object\",\n  \"description\": \"Snowflake parameter defined at the system, account, user, session, or object level.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter name.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter value.\"\n    },\n    \"defaultValue\": {\n      \"type\": \"string\",\n      \"description\": \"Default parameter value.\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the parameter value. Either BOOLEAN, NUMBER, FLOAT, or STRING.\"\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"description\": \"Level at which parameter is defined.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter description.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-parameter-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Parameter
---
