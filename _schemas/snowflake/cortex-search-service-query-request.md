---
description: A search query and additional parameters for search.
layout: schema
name: QueryRequest
properties_list:
- description: Unstructured text query. Exactly one of 'query' or 'multi_index_query' must be specified.
  name: query
  type: string
- description: A search query expressed as a collection of multiple column-level queries. Exactly one of 'query' or 'multi_index_query' must be specified. A column/index can be queried with multiple queries.
  name: multi_index_query
  type: object
- description: List of columns to return.
  name: columns
  type: array
- description: Filter query.
  name: filter
  type: object
- description: Max number of results to return.
  name: limit
  type: integer
- description: reserved
  name: experimental
  type: object
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-query-request-schema.json
slug: cortex-search-service-query-request
source_filename: cortex-search-service-query-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryRequest\",\n  \"type\": \"object\",\n  \"description\": \"A search query and additional parameters for search.\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Unstructured text query.  Exactly one of 'query' or 'multi_index_query' must be specified.\"\n    },\n    \"multi_index_query\": {\n      \"type\": \"object\",\n      \"description\": \"A search query expressed as a collection of multiple column-level queries.  Exactly one of 'query' or 'multi_index_query' must be specified. A column/index can be queried with multiple queries.\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"List of columns to return.\"\n    },\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"Filter query.\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Max number of results\
  \ to return.\"\n    },\n    \"experimental\": {\n      \"type\": \"object\",\n      \"description\": \"reserved\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-query-request-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: QueryRequest
---
