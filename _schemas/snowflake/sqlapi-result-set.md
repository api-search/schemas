---
description: ''
layout: schema
name: ResultSet
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
- description: Timestamp that specifies when the statement execution started.‌ The timestamp is expressed in milliseconds since the epoch.‌
  name: createdOn
  type: integer
- description: ''
  name: statementStatusUrl
  type: string
- description: ''
  name: resultSetMetaData
  type: object
- description: Result set data.
  name: data
  type: array
- description: these stats might not be available for each request.
  name: stats
  type: object
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/sqlapi-result-set-schema.json
slug: sqlapi-result-set
source_filename: sqlapi-result-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResultSet\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"sqlState\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"statementHandle\": {\n      \"type\": \"string\"\n    },\n    \"createdOn\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp that specifies when the statement execution started.\\u200c The timestamp is expressed in milliseconds since the epoch.\\u200c\"\n    },\n    \"statementStatusUrl\": {\n      \"type\": \"string\"\n    },\n    \"resultSetMetaData\": {\n      \"type\": \"object\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Result set data.\"\n    },\n    \"stats\": {\n      \"type\": \"object\",\n      \"description\": \"these stats might not be available for each request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/sqlapi-result-set-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ResultSet
---
