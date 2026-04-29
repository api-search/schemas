---
description: Specifies the schedule for periodically refreshing the dynamic table.
layout: schema
name: TargetLag
properties_list:
- description: Type of lag, can be either USER_DEFINED or DOWNSTREAM.
  name: type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-target-lag-schema.json
slug: common-target-lag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TargetLag\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the schedule for periodically refreshing the dynamic table.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of lag, can be either USER_DEFINED or DOWNSTREAM.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-target-lag-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TargetLag
---
