---
description: ''
layout: schema
name: ScheduleEntry
properties_list: []
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/scheduleentry-schema.json
slug: scheduleentry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/scheduleentry-schema.json\",\n  \"title\": \"ScheduleEntry\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Recording\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"summary\": {\n          \"type\": \"string\",\n          \"description\": \"Entry title/summary\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"HTML-formatted entry description\"\n        },\n        \"all_day\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is an all-day event\"\n        },\n        \"starts_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Entry start time in ISO 8601 format\"\n        },\n        \"ends_at\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\",\n          \"description\": \"Entry end time in ISO 8601 format\"\n        },\n        \"participants\": {\n          \"type\": \"array\",\n          \"description\": \"People participating in this entry\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/PersonRef\"\n          }\n        },\n        \"comments_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of comments on this entry\"\n        },\n        \"recurrence_schedule\": {\n          \"$ref\": \"#/components/schemas/RecurrenceSchedule\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/scheduleentry-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ScheduleEntry
---
