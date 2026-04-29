---
description: Status returned when a statement cancellation is requested.
layout: schema
name: CancelStatus
properties_list:
- description: Status code for the cancellation.
  name: code
  type: string
- description: SQL state code.
  name: sqlState
  type: string
- description: Message describing the cancellation status.
  name: message
  type: string
- description: Handle of the canceled statement.
  name: statementHandle
  type: string
- description: URL for checking the status of the canceled statement.
  name: statementStatusUrl
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/snowflake-sql-rest-cancel-status-schema.json
slug: snowflake-sql-rest-cancel-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CancelStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status returned when a statement cancellation is requested.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Status code for the cancellation.\"\n    },\n    \"sqlState\": {\n      \"type\": \"string\",\n      \"description\": \"SQL state code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Message describing the cancellation status.\"\n    },\n    \"statementHandle\": {\n      \"type\": \"string\",\n      \"description\": \"Handle of the canceled statement.\"\n    },\n    \"statementStatusUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL for checking the status of the canceled statement.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/snowflake-sql-rest-cancel-status-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: CancelStatus
---
