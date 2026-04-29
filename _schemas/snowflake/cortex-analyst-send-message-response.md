---
description: The non-streaming response object for the sendMessage
layout: schema
name: SendMessageResponse
properties_list:
- description: Unique request ID
  name: request_id
  type: string
- description: ''
  name: warnings
  type: array
- description: ''
  name: response_metadata
  type: object
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-send-message-response-schema.json
slug: cortex-analyst-send-message-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SendMessageResponse\",\n  \"type\": \"object\",\n  \"description\": \"The non-streaming response object for the sendMessage\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique request ID\"\n    },\n    \"warnings\": {\n      \"type\": \"array\"\n    },\n    \"response_metadata\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-send-message-response-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: SendMessageResponse
---
