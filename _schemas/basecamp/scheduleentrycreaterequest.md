---
description: ''
layout: schema
name: ScheduleEntryCreateRequest
properties_list:
- description: Entry title/summary
  name: summary
  type: string
- description: Entry start time in ISO 8601 format
  name: starts_at
  type: string
- description: Entry end time in ISO 8601 format
  name: ends_at
  type: string
- description: HTML-formatted entry description
  name: description
  type: string
- description: Person IDs to add as participants
  name: participant_ids
  type: array
- description: Whether this is an all-day event
  name: all_day
  type: boolean
- description: Whether to notify participants
  name: notify
  type: boolean
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/scheduleentrycreaterequest-schema.json
slug: scheduleentrycreaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/scheduleentrycreaterequest-schema.json\",\n  \"title\": \"ScheduleEntryCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"summary\",\n    \"starts_at\",\n    \"ends_at\"\n  ],\n  \"properties\": {\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Entry title/summary\"\n    },\n    \"starts_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Entry start time in ISO 8601 format\"\n    },\n    \"ends_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Entry end time in ISO 8601 format\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"HTML-formatted entry description\"\n    },\n    \"participant_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Person IDs to add as\
  \ participants\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"all_day\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an all-day event\"\n    },\n    \"notify\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to notify participants\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/scheduleentrycreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ScheduleEntryCreateRequest
---
