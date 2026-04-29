---
description: ''
layout: schema
name: Schedule
properties_list:
- description: The unique identifier for the schedule.
  name: id
  type: string
- description: The name of the schedule.
  name: name
  type: string
- description: Whether the schedule is active or suspended.
  name: state
  type: string
- description: The priority of the schedule (1-100). Lower numbers indicate higher priority.
  name: priority
  type: integer
- description: The date and time the schedule was created.
  name: createdAt
  type: string
- description: The date and time the schedule was last updated.
  name: updatedAt
  type: string
- description: The type of the schedule.
  name: type
  type: string
- description: How frequently the schedule runs.
  name: frequency
  type: string
- description: The next scheduled run time.
  name: nextRunAt
  type: string
- description: The time when the schedule ends.
  name: endScheduleAt
  type: string
- description: ''
  name: frequencyDetails
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-schedule-schema.json
slug: tableau-rest-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Schedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the schedule.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the schedule.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the schedule is active or suspended.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The priority of the schedule (1-100). Lower numbers indicate higher priority.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the schedule was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the schedule was last updated.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The type of the schedule.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"How frequently the schedule runs.\"\n    },\n    \"nextRunAt\": {\n      \"type\": \"string\",\n      \"description\": \"The next scheduled run time.\"\n    },\n    \"endScheduleAt\": {\n      \"type\": \"string\",\n      \"description\": \"The time when the schedule ends.\"\n    },\n    \"frequencyDetails\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-schedule-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Schedule
---
