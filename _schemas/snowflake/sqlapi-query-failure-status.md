---
description: ''
layout: schema
name: QueryFailureStatus
properties_list:
- description: ''
  name: code
  type: string
- description: ''
  name: sqlState
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: statementHandle
  type: string
- description: Timestamp that specifies when the statement execution started.‌ The timestamp is expressed in milliseconds since the epoch.
  name: createdOn
  type: integer
- description: ''
  name: statementStatusUrl
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/sqlapi-query-failure-status-schema.json
slug: sqlapi-query-failure-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryFailureStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"sqlState\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"statementHandle\": {\n      \"type\": \"string\"\n    },\n    \"createdOn\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp that specifies when the statement execution started.\\u200c The timestamp is expressed in milliseconds since the epoch.\"\n    },\n    \"statementStatusUrl\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/sqlapi-query-failure-status-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: QueryFailureStatus
---
