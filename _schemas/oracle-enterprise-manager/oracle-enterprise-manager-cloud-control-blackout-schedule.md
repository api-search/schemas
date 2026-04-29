---
description: Schedule definition for a blackout.
layout: schema
name: BlackoutSchedule
properties_list:
- description: Scheduled start time of the blackout.
  name: startTime
  type: string
- description: Scheduled end time of the blackout.
  name: endTime
  type: string
- description: Duration in minutes if no explicit end time is specified.
  name: duration
  type: integer
- description: Time zone for the schedule.
  name: timezone
  type: string
- description: Recurrence frequency for repeating blackouts.
  name: frequency
  type: string
- description: Interval for repeating blackouts (e.g., every 2 weeks).
  name: repeatInterval
  type: integer
- description: Days of the week for weekly recurrence.
  name: daysOfWeek
  type: array
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-blackout-schedule-schema.json
slug: oracle-enterprise-manager-cloud-control-blackout-schedule
source_filename: oracle-enterprise-manager-cloud-control-blackout-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlackoutSchedule\",\n  \"type\": \"object\",\n  \"description\": \"Schedule definition for a blackout.\",\n  \"properties\": {\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled start time of the blackout.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled end time of the blackout.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration in minutes if no explicit end time is specified.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone for the schedule.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Recurrence frequency for repeating blackouts.\"\n    },\n    \"repeatInterval\": {\n      \"type\": \"integer\",\n      \"description\": \"Interval for repeating blackouts (e.g., every 2 weeks).\"\
  \n    },\n    \"daysOfWeek\": {\n      \"type\": \"array\",\n      \"description\": \"Days of the week for weekly recurrence.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-blackout-schedule-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: BlackoutSchedule
---
