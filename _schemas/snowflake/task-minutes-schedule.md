---
description: A schedule for executing a task at specified intervals of minutes.
layout: schema
name: MinutesSchedule
properties_list:
- description: The number of minutes between each task run.
  name: minutes
  type: integer
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/task-minutes-schedule-schema.json
slug: task-minutes-schedule
source_filename: task-minutes-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MinutesSchedule\",\n  \"type\": \"object\",\n  \"description\": \"A schedule for executing a task at specified intervals of minutes.\",\n  \"properties\": {\n    \"minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of minutes between each task run.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/task-minutes-schedule-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: MinutesSchedule
---
