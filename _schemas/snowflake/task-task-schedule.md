---
description: Specifies the schedule for periodically running the task.
layout: schema
name: TaskSchedule
properties_list:
- description: Type of the schedule, can be either CRON_TYPE or MINUTES_TYPE.
  name: schedule_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/task-task-schedule-schema.json
slug: task-task-schedule
source_filename: task-task-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskSchedule\",\n  \"type\": \"object\",\n  \"description\": \"Specifies the schedule for periodically running the task.\",\n  \"properties\": {\n    \"schedule_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the schedule, can be either CRON_TYPE or MINUTES_TYPE.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/task-task-schedule-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: TaskSchedule
---
