---
description: Describes a date range over which a recurring event repeats.
layout: schema
name: RecurrenceRange
properties_list:
- description: The recurrence range type.
  name: type
  type: string
- description: The start date of the series (first occurrence).
  name: startDate
  type: string
- description: The date to stop applying the recurrence pattern.
  name: endDate
  type: string
- description: The number of times to repeat the event.
  name: numberOfOccurrences
  type: integer
- description: Time zone for the startDate and endDate properties.
  name: recurrenceTimeZone
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-recurrence-range-schema.json
slug: microsoft-graph-recurrence-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecurrenceRange\",\n  \"type\": \"object\",\n  \"description\": \"Describes a date range over which a recurring event repeats.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The recurrence range type.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The start date of the series (first occurrence).\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date to stop applying the recurrence pattern.\"\n    },\n    \"numberOfOccurrences\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times to repeat the event.\"\n    },\n    \"recurrenceTimeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone for the startDate and endDate properties.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-recurrence-range-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: RecurrenceRange
---
