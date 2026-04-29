---
description: ''
layout: schema
name: TimeClockEventRequest
properties_list:
- description: ''
  name: clockEventTime
  type: string
- description: ''
  name: timeZone
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/timeTracking-time-clock-event-request-schema.json
slug: timeTracking-time-clock-event-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeClockEventRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clockEventTime\": {\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/timeTracking-time-clock-event-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TimeClockEventRequest
---
