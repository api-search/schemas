---
description: A cron-based schedule for automatic workflow execution in Apache DolphinScheduler.
layout: schema
name: Schedule
properties_list:
- description: Schedule ID.
  name: id
  type: integer
- description: Workflow definition code to schedule.
  name: processDefinitionCode
  type: integer
- description: Cron expression for the schedule.
  name: crontab
  type: string
- description: Schedule start datetime.
  name: startTime
  type: string
- description: Schedule end datetime.
  name: endTime
  type: string
- description: Timezone for cron evaluation.
  name: timezoneId
  type: string
- description: Strategy on schedule failure.
  name: failureStrategy
  type: string
- description: When to send alerts.
  name: warningType
  type: string
- description: Whether this schedule is active.
  name: releaseState
  type: string
provider_name: Apache DolphinScheduler
provider_slug: apache-dolphinscheduler
schema_file: json-schema/apache-dolphinscheduler-schedule-schema.json
slug: apache-dolphinscheduler-schedule
source_filename: apache-dolphinscheduler-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dolphinscheduler/refs/heads/main/json-schema/apache-dolphinscheduler-schedule-schema.json\",\n  \"title\": \"Schedule\",\n  \"description\": \"A cron-based schedule for automatic workflow execution in Apache DolphinScheduler.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Schedule ID.\",\n      \"example\": 301\n    },\n    \"processDefinitionCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Workflow definition code to schedule.\",\n      \"example\": 8888888888888\n    },\n    \"crontab\": {\n      \"type\": \"string\",\n      \"description\": \"Cron expression for the schedule.\",\n      \"example\": \"0 0 1 * * ? *\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Schedule start\
  \ datetime.\",\n      \"example\": \"2025-01-01T00:00:00Z\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Schedule end datetime.\",\n      \"example\": \"2026-01-01T00:00:00Z\"\n    },\n    \"timezoneId\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for cron evaluation.\",\n      \"example\": \"America/Los_Angeles\"\n    },\n    \"failureStrategy\": {\n      \"type\": \"string\",\n      \"description\": \"Strategy on schedule failure.\",\n      \"enum\": [\n        \"CONTINUE\",\n        \"END\"\n      ],\n      \"example\": \"CONTINUE\"\n    },\n    \"warningType\": {\n      \"type\": \"string\",\n      \"description\": \"When to send alerts.\",\n      \"enum\": [\n        \"NONE\",\n        \"SUCCESS\",\n        \"FAILURE\",\n        \"ALL\"\n      ],\n      \"example\": \"FAILURE\"\n    },\n    \"releaseState\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this schedule is\
  \ active.\",\n      \"enum\": [\n        \"ONLINE\",\n        \"OFFLINE\"\n      ],\n      \"example\": \"ONLINE\"\n    }\n  },\n  \"required\": [\n    \"processDefinitionCode\",\n    \"crontab\",\n    \"startTime\",\n    \"endTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dolphinscheduler/refs/heads/main/json-schema/apache-dolphinscheduler-schedule-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: Schedule
---
