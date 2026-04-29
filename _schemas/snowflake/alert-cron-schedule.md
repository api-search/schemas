---
description: ''
layout: schema
name: CronSchedule
properties_list:
- description: A cron expression for the scheduled execution.
  name: cron_expr
  type: string
- description: The time zone for the schedule.
  name: timezone
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/alert-cron-schedule-schema.json
slug: alert-cron-schedule
source_filename: alert-cron-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CronSchedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cron_expr\": {\n      \"type\": \"string\",\n      \"description\": \"A cron expression for the scheduled execution.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone for the schedule.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/alert-cron-schedule-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: CronSchedule
---
