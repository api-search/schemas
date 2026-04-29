---
description: ''
layout: schema
name: PointOfTimeStream
properties_list:
- description: Creates the new stream at the same offset as the specified stream.
  name: stream
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stream-point-of-time-stream-schema.json
slug: stream-point-of-time-stream
source_filename: stream-point-of-time-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PointOfTimeStream\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stream\": {\n      \"type\": \"string\",\n      \"description\": \"Creates the new stream at the same offset as the specified stream. \"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stream-point-of-time-stream-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PointOfTimeStream
---
