---
description: ''
layout: schema
name: ScheduleUpdate
properties_list:
- description: The updated start time in HH:MM format.
  name: start_time
  type: string
- description: The updated maximum number of guests for this session.
  name: max_guests
  type: integer
- description: The updated status of the schedule entry.
  name: status
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-schedule-update-schema.json
slug: airbnb-schedule-update
source_filename: airbnb-schedule-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-schedule-update-schema.json\",\n  \"title\": \"ScheduleUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"The updated start time in HH:MM format.\",\n      \"pattern\": \"^[0-2][0-9]:[0-5][0-9]$\"\n    },\n    \"max_guests\": {\n      \"type\": \"integer\",\n      \"description\": \"The updated maximum number of guests for this session.\",\n      \"minimum\": 1\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The updated status of the schedule entry.\",\n      \"enum\": [\n        \"open\",\n        \"cancelled\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-schedule-update-schema.json
tags: []
title: ScheduleUpdate
---
