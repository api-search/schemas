---
description: Point of time identified by a timestamp.
layout: schema
name: PointOfTimeTimestamp
properties_list:
- description: Timestamp of the point of time.
  name: timestamp
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-point-of-time-timestamp-schema.json
slug: common-point-of-time-timestamp
source_filename: common-point-of-time-timestamp-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PointOfTimeTimestamp\",\n  \"type\": \"object\",\n  \"description\": \"Point of time identified by a timestamp.\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the point of time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-point-of-time-timestamp-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PointOfTimeTimestamp
---
