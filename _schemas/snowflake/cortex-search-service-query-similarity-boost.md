---
description: ''
layout: schema
name: QuerySimilarityBoost
properties_list:
- description: Fully-qualified name of a Cortex Search Service through which to find similar previous queries.
  name: cortex_search_service
  type: string
- description: Name of a TEXT column indexed in the specified previous queries search service that contains the previous query strings.
  name: previous_query_column
  type: string
- description: Name of an ARRAY column indexed in the specified previous queries search service that contains a list of documents that matched the corresponding previous query. Each document is represented as an OBJ
  name: documents_column
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-query-similarity-boost-schema.json
slug: cortex-search-service-query-similarity-boost
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QuerySimilarityBoost\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cortex_search_service\": {\n      \"type\": \"string\",\n      \"description\": \"Fully-qualified name of a Cortex Search Service through which to find similar previous queries.\"\n    },\n    \"previous_query_column\": {\n      \"type\": \"string\",\n      \"description\": \"Name of a TEXT column indexed in the specified previous queries search service that contains the previous query strings.\"\n    },\n    \"documents_column\": {\n      \"type\": \"string\",\n      \"description\": \"Name of an ARRAY column indexed in the specified previous queries search service that contains a list of documents that matched the corresponding previous query. Each document is represented as an OBJECT mapping all primary key columns to their corresponding values.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-query-similarity-boost-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: QuerySimilarityBoost
---
