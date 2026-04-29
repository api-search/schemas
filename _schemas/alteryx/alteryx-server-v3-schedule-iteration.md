---
description: Schedule iteration configuration defining when and how often a schedule runs
layout: schema
name: ScheduleIteration
properties_list:
- description: The frequency pattern for the schedule
  name: iterationType
  type: string
- description: Start date and time (ISO 8601, must be in the future)
  name: startTime
  type: string
- description: End date and time (ISO 8601)
  name: endTime
  type: string
- description: Configuration for hourly iteration
  name: hourlyContract
  type: object
- description: Configuration for daily iteration
  name: dailyContract
  type: object
- description: Configuration for weekly iteration
  name: weeklyContract
  type: object
- description: Configuration for monthly iteration
  name: monthlyContract
  type: object
- description: Configuration for custom iteration
  name: customContract
  type: object
- description: Configuration for cron-based iteration
  name: cronContract
  type: object
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-schedule-iteration-schema.json
slug: alteryx-server-v3-schedule-iteration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScheduleIteration\",\n  \"type\": \"object\",\n  \"description\": \"Schedule iteration configuration defining when and how often a schedule runs\",\n  \"properties\": {\n    \"iterationType\": {\n      \"type\": \"string\",\n      \"description\": \"The frequency pattern for the schedule\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Start date and time (ISO 8601, must be in the future)\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"End date and time (ISO 8601)\"\n    },\n    \"hourlyContract\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for hourly iteration\"\n    },\n    \"dailyContract\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for daily iteration\"\n    },\n    \"weeklyContract\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for\
  \ weekly iteration\"\n    },\n    \"monthlyContract\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for monthly iteration\"\n    },\n    \"customContract\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for custom iteration\"\n    },\n    \"cronContract\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for cron-based iteration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-schedule-iteration-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: ScheduleIteration
---
