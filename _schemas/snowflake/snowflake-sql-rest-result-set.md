---
description: The result set returned from a successfully executed SQL statement, including metadata, row data, and execution statistics.
layout: schema
name: ResultSet
properties_list:
- description: Status code for the query.
  name: code
  type: string
- description: SQL state code.
  name: sqlState
  type: string
- description: Message describing the execution status.
  name: message
  type: string
- description: Handle that uniquely identifies the executed statement.
  name: statementHandle
  type: string
- description: Timestamp that specifies when the statement execution started. The timestamp is expressed in milliseconds since the epoch.
  name: createdOn
  type: integer
- description: URL for checking the status of the statement.
  name: statementStatusUrl
  type: string
- description: Result set data. Each element in the outer array represents a row. Each element in the inner array represents a column value as a string.
  name: data
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-result-set-schema.json
slug: snowflake-sql-rest-result-set
source_filename: snowflake-sql-rest-result-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResultSet\",\n  \"type\": \"object\",\n  \"description\": \"The result set returned from a successfully executed SQL statement, including metadata, row data, and execution statistics.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Status code for the query.\"\n    },\n    \"sqlState\": {\n      \"type\": \"string\",\n      \"description\": \"SQL state code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Message describing the execution status.\"\n    },\n    \"statementHandle\": {\n      \"type\": \"string\",\n      \"description\": \"Handle that uniquely identifies the executed statement.\"\n    },\n    \"createdOn\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp that specifies when the statement execution started. The timestamp is expressed in milliseconds since the epoch.\"\n    },\n\
  \    \"statementStatusUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL for checking the status of the statement.\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Result set data. Each element in the outer array represents a row. Each element in the inner array represents a column value as a string.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-result-set-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ResultSet
---
