---
description: ''
layout: schema
name: StreamingError
properties_list:
- description: A description of the error
  name: message
  type: string
- description: The Snowflake error code categorizing the error
  name: code
  type: string
- description: Unique request ID
  name: request_id
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-streaming-error-schema.json
slug: cortex-analyst-streaming-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StreamingError\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the error\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The Snowflake error code categorizing the error\"\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique request ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-streaming-error-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StreamingError
---
