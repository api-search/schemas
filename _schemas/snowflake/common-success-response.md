---
description: Schema for all the success responses returned by the server.
layout: schema
name: SuccessResponse
properties_list:
- description: Message returned by the server.
  name: status
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-success-response-schema.json
slug: common-success-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessResponse\",\n  \"type\": \"object\",\n  \"description\": \"Schema for all the success responses returned by the server.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Message returned by the server.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-success-response-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: SuccessResponse
---
