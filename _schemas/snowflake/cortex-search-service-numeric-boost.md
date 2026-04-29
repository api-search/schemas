---
description: ''
layout: schema
name: NumericBoost
properties_list:
- description: Weight to apply for boosting this numerical column. It will be normalized across all scored columns specified in the scoring config so that all weights sum to 1. If a weight is not provided, the weigh
  name: weight
  type: number
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-numeric-boost-schema.json
slug: cortex-search-service-numeric-boost
source_filename: cortex-search-service-numeric-boost-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NumericBoost\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Weight to apply for boosting this numerical column. It will be normalized across all scored columns specified in the scoring config so that all weights sum to 1. If a weight is not provided, the weight defaults to 1 pre-normalization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-numeric-boost-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NumericBoost
---
