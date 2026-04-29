---
description: Functions to apply for scoring this request.
layout: schema
name: Functions
properties_list:
- description: ''
  name: numeric_boosts
  type: array
- description: ''
  name: time_decays
  type: array
- description: ''
  name: text_boosts
  type: array
- description: ''
  name: vector_boosts
  type: array
- description: ''
  name: query_similarity_boosts
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-functions-schema.json
slug: cortex-search-service-functions
source_filename: cortex-search-service-functions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Functions\",\n  \"type\": \"object\",\n  \"description\": \"Functions to apply for scoring this request.\",\n  \"properties\": {\n    \"numeric_boosts\": {\n      \"type\": \"array\"\n    },\n    \"time_decays\": {\n      \"type\": \"array\"\n    },\n    \"text_boosts\": {\n      \"type\": \"array\"\n    },\n    \"vector_boosts\": {\n      \"type\": \"array\"\n    },\n    \"query_similarity_boosts\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-functions-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Functions
---
