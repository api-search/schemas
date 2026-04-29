---
description: ''
layout: schema
name: PointOfTime
properties_list:
- description: 'Type of the point of time. Possible values include: timestamp, offset, statement'
  name: point_of_time_type
  type: string
- description: Relation to the point of time. Currently, the API supports `at` and `before`
  name: reference
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/stream-point-of-time-schema.json
slug: stream-point-of-time
source_filename: stream-point-of-time-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PointOfTime\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"point_of_time_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the point of time. Possible values include: timestamp, offset, statement\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Relation to the point of time.  Currently, the API supports `at` and `before`\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/stream-point-of-time-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PointOfTime
---
