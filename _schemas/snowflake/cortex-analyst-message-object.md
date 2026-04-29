---
description: Represents a message within a chat.
layout: schema
name: MessageObject
properties_list:
- description: The entity that produced the message. One of `user` or `analyst`.
  name: role
  type: string
- description: The content of the message in array of text or SQL.
  name: content
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-message-object-schema.json
slug: cortex-analyst-message-object
source_filename: cortex-analyst-message-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageObject\",\n  \"type\": \"object\",\n  \"description\": \"Represents a message within a chat.\",\n  \"properties\": {\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The entity that produced the message. One of `user` or `analyst`.\"\n    },\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The content of the message in array of text or SQL.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-message-object-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: MessageObject
---
