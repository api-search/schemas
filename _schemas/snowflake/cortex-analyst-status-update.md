---
description: ''
layout: schema
name: StatusUpdate
properties_list:
- description: The latest status for processing the request
  name: status
  type: string
- description: A human readable description on the current request processing status
  name: status_message
  type: string
- description: Unique request ID.
  name: request_id
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-status-update-schema.json
slug: cortex-analyst-status-update
source_filename: cortex-analyst-status-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatusUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The latest status for processing the request\"\n    },\n    \"status_message\": {\n      \"type\": \"string\",\n      \"description\": \"A human readable description on the current request processing status\"\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique request ID.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-status-update-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StatusUpdate
---
