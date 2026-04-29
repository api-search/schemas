---
description: User-defined target lag.
layout: schema
name: UserDefinedLag
properties_list:
- description: Target lag time in seconds.
  name: seconds
  type: integer
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-user-defined-lag-schema.json
slug: common-user-defined-lag
source_filename: common-user-defined-lag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserDefinedLag\",\n  \"type\": \"object\",\n  \"description\": \"User-defined target lag.\",\n  \"properties\": {\n    \"seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Target lag time in seconds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-user-defined-lag-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: UserDefinedLag
---
