---
description: Describes the frequency by which a recurring event repeats.
layout: schema
name: RecurrencePattern
properties_list:
- description: The recurrence pattern type.
  name: type
  type: string
- description: The number of units between occurrences, where units can be in days, weeks, months, or years.
  name: interval
  type: integer
- description: A collection of the days of the week on which the event occurs.
  name: daysOfWeek
  type: array
- description: The day of the month on which the event occurs.
  name: dayOfMonth
  type: integer
- description: The month in which the event occurs (1-12).
  name: month
  type: integer
- description: The first day of the week.
  name: firstDayOfWeek
  type: string
- description: The week index for relative monthly and yearly patterns.
  name: index
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-recurrence-pattern-schema.json
slug: microsoft-graph-recurrence-pattern
source_filename: microsoft-graph-recurrence-pattern-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecurrencePattern\",\n  \"type\": \"object\",\n  \"description\": \"Describes the frequency by which a recurring event repeats.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The recurrence pattern type.\"\n    },\n    \"interval\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of units between occurrences, where units can be in days, weeks, months, or years.\"\n    },\n    \"daysOfWeek\": {\n      \"type\": \"array\",\n      \"description\": \"A collection of the days of the week on which the event occurs.\"\n    },\n    \"dayOfMonth\": {\n      \"type\": \"integer\",\n      \"description\": \"The day of the month on which the event occurs.\"\n    },\n    \"month\": {\n      \"type\": \"integer\",\n      \"description\": \"The month in which the event occurs (1-12).\"\n    },\n    \"firstDayOfWeek\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"The first day of the week.\"\n    },\n    \"index\": {\n      \"type\": \"string\",\n      \"description\": \"The week index for relative monthly and yearly patterns.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-recurrence-pattern-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: RecurrencePattern
---
