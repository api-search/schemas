---
description: Session parameters that should be set before executing the statement.
layout: schema
name: SessionParameters
properties_list:
- description: Time zone to use when executing the statement.
  name: timezone
  type: string
- description: Query tag that you want to associate with the SQL statement.
  name: query_tag
  type: string
- description: Output format for binary values.
  name: binary_output_format
  type: string
- description: Output format for DATE values.
  name: date_output_format
  type: string
- description: Output format for TIME values.
  name: time_output_format
  type: string
- description: Output format for TIMESTAMP values.
  name: timestamp_output_format
  type: string
- description: Output format for TIMESTAMP_LTZ values.
  name: timestamp_ltz_output_format
  type: string
- description: Output format for TIMESTAMP_NTZ values.
  name: timestamp_ntz_output_format
  type: string
- description: Output format for TIMESTAMP_TZ values.
  name: timestamp_tz_output_format
  type: string
- description: Number of statements to execute when using multi-statement capability. 0 implies variable number of statements. Negative numbers are not allowed.
  name: multi_statement_count
  type: integer
- description: Maximum size of each set (chunk) of query results to download.
  name: client_result_chunk_size
  type: integer
- description: Maximum number of rows returned in a result set.
  name: rows_per_resultset
  type: integer
- description: Whether to use a previously-cached result set for a query whose result set is still in the cache.
  name: use_cached_result
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-session-parameters-schema.json
slug: snowflake-sql-rest-session-parameters
source_filename: snowflake-sql-rest-session-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SessionParameters\",\n  \"type\": \"object\",\n  \"description\": \"Session parameters that should be set before executing the statement.\",\n  \"properties\": {\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone to use when executing the statement.\"\n    },\n    \"query_tag\": {\n      \"type\": \"string\",\n      \"description\": \"Query tag that you want to associate with the SQL statement.\"\n    },\n    \"binary_output_format\": {\n      \"type\": \"string\",\n      \"description\": \"Output format for binary values.\"\n    },\n    \"date_output_format\": {\n      \"type\": \"string\",\n      \"description\": \"Output format for DATE values.\"\n    },\n    \"time_output_format\": {\n      \"type\": \"string\",\n      \"description\": \"Output format for TIME values.\"\n    },\n    \"timestamp_output_format\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Output format for TIMESTAMP values.\"\n    },\n    \"timestamp_ltz_output_format\": {\n      \"type\": \"string\",\n      \"description\": \"Output format for TIMESTAMP_LTZ values.\"\n    },\n    \"timestamp_ntz_output_format\": {\n      \"type\": \"string\",\n      \"description\": \"Output format for TIMESTAMP_NTZ values.\"\n    },\n    \"timestamp_tz_output_format\": {\n      \"type\": \"string\",\n      \"description\": \"Output format for TIMESTAMP_TZ values.\"\n    },\n    \"multi_statement_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of statements to execute when using multi-statement capability. 0 implies variable number of statements. Negative numbers are not allowed.\"\n    },\n    \"client_result_chunk_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum size of each set (chunk) of query results to download.\"\n    },\n    \"rows_per_resultset\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of\
  \ rows returned in a result set.\"\n    },\n    \"use_cached_result\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use a previously-cached result set for a query whose result set is still in the cache.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-session-parameters-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: SessionParameters
---
