---
description: ''
layout: schema
name: TextBoost
properties_list:
- description: Weight to apply for boosting this text column.
  name: weight
  type: number
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-text-boost-schema.json
slug: cortex-search-service-text-boost
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TextBoost\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Weight to apply for boosting this text column.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-text-boost-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TextBoost
---
