---
description: ''
layout: schema
name: VectorBoost
properties_list:
- description: Weight to apply for boosting this vector column.
  name: weight
  type: number
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-vector-boost-schema.json
slug: cortex-search-service-vector-boost
source_filename: cortex-search-service-vector-boost-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VectorBoost\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Weight to apply for boosting this vector column.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-vector-boost-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: VectorBoost
---
