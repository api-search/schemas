---
description: ''
layout: schema
name: Schedule
properties_list:
- description: Type of the schedule, can be either CRON_TYPE or MINUTES_TYPE
  name: schedule_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/alert-schedule-schema.json
slug: alert-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Schedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schedule_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the schedule, can be either CRON_TYPE or MINUTES_TYPE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/alert-schedule-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Schedule
---
