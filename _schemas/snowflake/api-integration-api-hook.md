---
description: ''
layout: schema
name: ApiHook
properties_list:
- description: Type of ApiHook, can be AWS, AZURE, GC or GIT.
  name: type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/api-integration-api-hook-schema.json
slug: api-integration-api-hook
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiHook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of ApiHook, can be AWS, AZURE, GC or GIT.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/api-integration-api-hook-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ApiHook
---
