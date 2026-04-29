---
description: Status returned when a query execution fails.
layout: schema
name: QueryFailureStatus
properties_list:
- description: Error code for the query failure.
  name: code
  type: string
- description: SQL state code indicating the error category.
  name: sqlState
  type: string
- description: Error message describing the failure.
  name: message
  type: string
- description: Handle that uniquely identifies the failed statement.
  name: statementHandle
  type: string
- description: Timestamp that specifies when the statement execution started. The timestamp is expressed in milliseconds since the epoch.
  name: createdOn
  type: integer
- description: URL for checking the status of the failed statement.
  name: statementStatusUrl
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-query-failure-status-schema.json
slug: snowflake-sql-rest-query-failure-status
source_filename: snowflake-sql-rest-query-failure-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryFailureStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status returned when a query execution fails.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code for the query failure.\"\n    },\n    \"sqlState\": {\n      \"type\": \"string\",\n      \"description\": \"SQL state code indicating the error category.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message describing the failure.\"\n    },\n    \"statementHandle\": {\n      \"type\": \"string\",\n      \"description\": \"Handle that uniquely identifies the failed statement.\"\n    },\n    \"createdOn\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp that specifies when the statement execution started. The timestamp is expressed in milliseconds since the epoch.\"\n    },\n    \"statementStatusUrl\": {\n   \
  \   \"type\": \"string\",\n      \"description\": \"URL for checking the status of the failed statement.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-query-failure-status-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: QueryFailureStatus
---
