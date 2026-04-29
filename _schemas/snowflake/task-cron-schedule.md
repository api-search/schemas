---
description: A cron schedule for executing a task at a specified interval.
layout: schema
name: CronSchedule
properties_list:
- description: A cron expression for the task execution.
  name: cron_expr
  type: string
- description: The time zone for the schedule.
  name: timezone
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/task-cron-schedule-schema.json
slug: task-cron-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CronSchedule\",\n  \"type\": \"object\",\n  \"description\": \"A cron schedule for executing a task at a specified interval.\",\n  \"properties\": {\n    \"cron_expr\": {\n      \"type\": \"string\",\n      \"description\": \"A cron expression for the task execution.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone for the schedule.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/task-cron-schedule-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: CronSchedule
---
