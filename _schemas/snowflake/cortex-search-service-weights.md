---
description: Weights to apply to each scoring component.
layout: schema
name: Weights
properties_list:
- description: Weight to apply to all text-specific columns.
  name: texts
  type: number
- description: Weight to apply to all vector-specific columns.
  name: vectors
  type: number
- description: Weight to apply to reranker-specific scoring component.
  name: reranker
  type: number
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-weights-schema.json
slug: cortex-search-service-weights
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Weights\",\n  \"type\": \"object\",\n  \"description\": \"Weights to apply to each scoring component.\",\n  \"properties\": {\n    \"texts\": {\n      \"type\": \"number\",\n      \"description\": \"Weight to apply to all text-specific columns.\"\n    },\n    \"vectors\": {\n      \"type\": \"number\",\n      \"description\": \"Weight to apply to all vector-specific columns.\"\n    },\n    \"reranker\": {\n      \"type\": \"number\",\n      \"description\": \"Weight to apply to reranker-specific scoring component.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-weights-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Weights
---
