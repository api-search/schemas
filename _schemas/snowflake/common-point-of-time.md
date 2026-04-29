---
description: Point of time.
layout: schema
name: PointOfTime
properties_list:
- description: 'Type of the point of time. Possible values include: - `timestamp`: Exact time using the standard timezone format. Example: `2023-09-15 10:59:43`. - `offset`: Interval relative to ''now.'' Example: `1 da'
  name: point_of_time_type
  type: string
- description: Relation to the point of time. Currently, the API supports `at` and `before`.
  name: reference
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-point-of-time-schema.json
slug: common-point-of-time
source_filename: common-point-of-time-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PointOfTime\",\n  \"type\": \"object\",\n  \"description\": \"Point of time.\",\n  \"properties\": {\n    \"point_of_time_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the point of time. Possible values include:\\n- `timestamp`: Exact time using the standard timezone format. Example: `2023-09-15 10:59:43`. - `offset`: Interval relative to 'now.' Example: `1 day`. - `statement`: ID of a query statement to use as the reference point for <a href=https://docs.snowflake.com/en/sql-reference/sql/create-clone#time-travel-parameters>Time Travel</a>.\\nFor more information, see https://docs.snowflake.com/en/sql-reference/data-types-datetime.\"\n    },\n    \"reference\": {\n      \"type\": \"string\",\n      \"description\": \"Relation to the point of time. Currently, the API supports `at` and `before`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-point-of-time-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PointOfTime
---
