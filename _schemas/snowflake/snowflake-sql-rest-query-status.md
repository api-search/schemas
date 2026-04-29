---
description: Status of a query that is in progress or has completed successfully.
layout: schema
name: QueryStatus
properties_list:
- description: Status code for the query execution.
  name: code
  type: string
- description: SQL state code.
  name: sqlState
  type: string
- description: Message describing the status of the query.
  name: message
  type: string
- description: Handle that uniquely identifies the statement. You can use this handle to check the status of the statement and retrieve the result set.
  name: statementHandle
  type: string
- description: Timestamp that specifies when the statement execution started. The timestamp is expressed in milliseconds since the epoch.
  name: createdOn
  type: integer
- description: URL that you can use to check the status of the execution of the statement and retrieve the result set.
  name: statementStatusUrl
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-query-status-schema.json
slug: snowflake-sql-rest-query-status
source_filename: snowflake-sql-rest-query-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status of a query that is in progress or has completed successfully.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Status code for the query execution.\"\n    },\n    \"sqlState\": {\n      \"type\": \"string\",\n      \"description\": \"SQL state code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Message describing the status of the query.\"\n    },\n    \"statementHandle\": {\n      \"type\": \"string\",\n      \"description\": \"Handle that uniquely identifies the statement. You can use this handle to check the status of the statement and retrieve the result set.\"\n    },\n    \"createdOn\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp that specifies when the statement execution started. The timestamp is expressed in\
  \ milliseconds since the epoch.\"\n    },\n    \"statementStatusUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL that you can use to check the status of the execution of the statement and retrieve the result set.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-query-status-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: QueryStatus
---
