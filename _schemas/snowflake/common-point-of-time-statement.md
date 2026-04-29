---
description: Point of time indicating when a statement was executed.
layout: schema
name: PointOfTimeStatement
properties_list:
- description: Statement of the point of time.
  name: statement
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/common-point-of-time-statement-schema.json
slug: common-point-of-time-statement
source_filename: common-point-of-time-statement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PointOfTimeStatement\",\n  \"type\": \"object\",\n  \"description\": \"Point of time indicating when a statement was executed.\",\n  \"properties\": {\n    \"statement\": {\n      \"type\": \"string\",\n      \"description\": \"Statement of the point of time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/common-point-of-time-statement-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: PointOfTimeStatement
---
