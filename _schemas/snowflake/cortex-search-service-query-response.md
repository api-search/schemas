---
description: Search results.
layout: schema
name: QueryResponse
properties_list:
- description: List of result rows.
  name: results
  type: array
- description: ID of the request.
  name: request_id
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-search-service-query-response-schema.json
slug: cortex-search-service-query-response
source_filename: cortex-search-service-query-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryResponse\",\n  \"type\": \"object\",\n  \"description\": \"Search results.\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"List of result rows.\"\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-search-service-query-response-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: QueryResponse
---
