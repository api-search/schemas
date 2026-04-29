---
description: A Snowflake stream
layout: schema
name: Stream
properties_list:
- description: Date and time when the stream was created.
  name: created_on
  type: string
- description: Name of the stream
  name: name
  type: string
- description: user comment associated to an object in the dictionary
  name: comment
  type: string
- description: Database in which the stream is stored
  name: database_name
  type: string
- description: Schema in which the stream is stored
  name: schema_name
  type: string
- description: Role that owns the stream
  name: owner
  type: string
- description: Table name whose changes are tracked by the stream
  name: table_name
  type: string
- description: Specifies whether the stream is stale or not
  name: stale
  type: boolean
- description: 'Mode of the stream. Possible values include: APPEND_ONLY, INSERT_ONLY. For streams on tables, the column displays DEFAULT.'
  name: mode
  type: string
- description: Timestamp when the stream became stale or may become stale if not consumed.
  name: stale_after
  type: string
- description: Reason why the stream cannot be queried successfully. This column supports future functionality. Currently, the only value returned is N/A.
  name: invalid_reason
  type: string
- description: The type of role that owns the stream
  name: owner_role_type
  type: string
- description: Type of the stream; currently DELTA only.
  name: type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stream-stream-schema.json
slug: stream-stream
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Stream\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake stream\",\n  \"properties\": {\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the stream was created.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the stream\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"user comment associated to an object in the dictionary\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database in which the stream is stored\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the stream is stored\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the stream\"\n    },\n    \"table_name\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Table name whose changes are tracked by the stream\"\n    },\n    \"stale\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the stream is stale or not\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"Mode of the stream. Possible values include: APPEND_ONLY, INSERT_ONLY. For streams on tables, the column displays DEFAULT.\"\n    },\n    \"stale_after\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the stream became stale or may become stale if not consumed. \"\n    },\n    \"invalid_reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason why the stream cannot be queried successfully. This column supports future functionality. Currently, the only value returned is N/A.\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the stream\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Type of the stream; currently DELTA only.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stream-stream-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Stream
---
