---
description: ''
layout: schema
name: TimeClockEvent
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The type of event (e.g., Clock In, Clock Out, Meal Start, Meal End).
  name: clockEventType
  type: string
- description: ''
  name: clockEventTime
  type: string
- description: ''
  name: timeZone
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/timeTracking-time-clock-event-schema.json
slug: timeTracking-time-clock-event
source_filename: timeTracking-time-clock-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeClockEvent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"clockEventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event (e.g., Clock In, Clock Out, Meal Start, Meal End).\"\n    },\n    \"clockEventTime\": {\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/timeTracking-time-clock-event-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TimeClockEvent
---
