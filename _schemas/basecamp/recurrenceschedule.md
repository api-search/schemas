---
description: Recurrence configuration for a schedule entry
layout: schema
name: RecurrenceSchedule
properties_list:
- description: Recurrence frequency
  name: frequency
  type: string
- description: Days of the week for weekly recurrence
  name: days
  type: array
- description: Hour of the day for the recurrence
  name: hour
  type: integer
- description: Minute of the hour for the recurrence
  name: minute
  type: integer
- description: Week instance within the month for monthly recurrence
  name: week_instance
  type: integer
- description: Date when the recurrence starts
  name: start_date
  type: string
- description: Date when the recurrence ends
  name: end_date
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/recurrenceschedule-schema.json
slug: recurrenceschedule
source_filename: recurrenceschedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/recurrenceschedule-schema.json\",\n  \"title\": \"RecurrenceSchedule\",\n  \"type\": \"object\",\n  \"description\": \"Recurrence configuration for a schedule entry\",\n  \"properties\": {\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Recurrence frequency\",\n      \"enum\": [\n        \"daily\",\n        \"weekly\",\n        \"monthly\",\n        \"yearly\"\n      ]\n    },\n    \"days\": {\n      \"type\": \"array\",\n      \"description\": \"Days of the week for weekly recurrence\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"hour\": {\n      \"type\": \"integer\",\n      \"description\": \"Hour of the day for the recurrence\"\n    },\n    \"minute\": {\n      \"type\": \"integer\",\n      \"description\": \"Minute of the hour for the recurrence\"\n    },\n    \"week_instance\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Week instance within the month for monthly recurrence\",\n      \"nullable\": true\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the recurrence starts\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the recurrence ends\",\n      \"nullable\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/recurrenceschedule-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: RecurrenceSchedule
---
