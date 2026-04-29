---
description: Query specification of a given column. Exactly one of 'text' or 'vector' must be specified.
layout: schema
name: ColumnQuery
properties_list:
- description: Unstructured text query for querying a text index.
  name: text
  type: string
- description: Query embedding vector. Must be computed using the same model as used for embedding the column being queried.
  name: vector
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-column-query-schema.json
slug: cortex-search-service-column-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ColumnQuery\",\n  \"type\": \"object\",\n  \"description\": \"Query specification of a given column. Exactly one of 'text' or 'vector' must be specified.\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Unstructured text query for querying a text index.\"\n    },\n    \"vector\": {\n      \"type\": \"array\",\n      \"description\": \"Query embedding vector. Must be computed using the same model as used for embedding the column being queried.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-column-query-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ColumnQuery
---
