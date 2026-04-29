---
description: ''
layout: schema
name: PointOfTimeOffset
properties_list:
- description: Point of time identified by an offset in reference to the current time, such as `10 min`.
  name: offset
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stream-point-of-time-offset-schema.json
slug: stream-point-of-time-offset
source_filename: stream-point-of-time-offset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PointOfTimeOffset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"offset\": {\n      \"type\": \"string\",\n      \"description\": \"Point of time identified by an offset in reference to the current time, such as `10 min`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stream-point-of-time-offset-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PointOfTimeOffset
---
