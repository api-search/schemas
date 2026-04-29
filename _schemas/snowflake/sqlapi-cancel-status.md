---
description: ''
layout: schema
name: CancelStatus
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
- description: ''
  name: statementStatusUrl
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/sqlapi-cancel-status-schema.json
slug: sqlapi-cancel-status
source_filename: sqlapi-cancel-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CancelStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"sqlState\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"statementHandle\": {\n      \"type\": \"string\"\n    },\n    \"statementStatusUrl\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/sqlapi-cancel-status-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: CancelStatus
---
