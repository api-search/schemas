---
description: ''
layout: schema
name: StreamSourceView
properties_list:
- description: Whether this stream is an append only stream or not
  name: append_only
  type: boolean
- description: Whether this stream show initial rows on first consumption
  name: show_initial_rows
  type: boolean
- description: List of base tables for the stream
  name: base_tables
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stream-stream-source-view-schema.json
slug: stream-stream-source-view
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StreamSourceView\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"append_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this stream is an append only stream or not\"\n    },\n    \"show_initial_rows\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this stream show initial rows on first consumption\"\n    },\n    \"base_tables\": {\n      \"type\": \"array\",\n      \"description\": \"List of base tables for the stream\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stream-stream-source-view-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: StreamSourceView
---
