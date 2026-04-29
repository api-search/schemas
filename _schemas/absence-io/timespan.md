---
description: A working time configuration defining work hours and schedule.
layout: schema
name: Timespan
properties_list:
- description: Unique identifier of the timespan.
  name: _id
  type: string
- description: Name of the working time configuration.
  name: name
  type: string
- description: Number of working hours per day.
  name: hoursPerDay
  type: number
- description: Number of working days per week.
  name: daysPerWeek
  type: integer
provider_name: Absence.io
provider_slug: absence-io
schema_file: json-schema/timespan-schema.json
slug: timespan
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/timespan-schema.json\",\n  \"title\": \"Timespan\",\n  \"description\": \"A working time configuration defining work hours and schedule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the timespan.\",\n      \"example\": \"500567\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the working time configuration.\",\n      \"example\": \"Standard Work Week\"\n    },\n    \"hoursPerDay\": {\n      \"type\": \"number\",\n      \"description\": \"Number of working hours per day.\",\n      \"example\": 8\n    },\n    \"daysPerWeek\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of working days per week.\",\n      \"example\": 5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/absence-io/refs/heads/main/json-schema/timespan-schema.json
tags:
- Absences
- Employees
- Leave Management
- HR
title: Timespan
---
