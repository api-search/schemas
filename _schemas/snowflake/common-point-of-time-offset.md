---
description: Point of time identified by an offset in reference to the current time, such as `10 min`.
layout: schema
name: PointOfTimeOffset
properties_list:
- description: 'Offset from the point of time. Example: `1 year`'
  name: offset
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-point-of-time-offset-schema.json
slug: common-point-of-time-offset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PointOfTimeOffset\",\n  \"type\": \"object\",\n  \"description\": \"Point of time identified by an offset in reference to the current time, such as `10 min`.\",\n  \"properties\": {\n    \"offset\": {\n      \"type\": \"string\",\n      \"description\": \"Offset from the point of time. Example: `1 year`\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-point-of-time-offset-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PointOfTimeOffset
---
