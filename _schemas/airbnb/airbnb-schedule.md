---
description: ''
layout: schema
name: Schedule
properties_list:
- description: The unique identifier of the schedule entry.
  name: id
  type: string
- description: The identifier of the associated experience.
  name: experience_id
  type: string
- description: The date of the scheduled session.
  name: date
  type: string
- description: The start time in HH:MM format.
  name: start_time
  type: string
- description: The end time in HH:MM format.
  name: end_time
  type: string
- description: The maximum number of guests for this session.
  name: max_guests
  type: integer
- description: The current number of booked guests.
  name: booked_guests
  type: integer
- description: The number of remaining available spots.
  name: available_spots
  type: integer
- description: The status of the schedule entry.
  name: status
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-schedule-schema.json
slug: airbnb-schedule
source_filename: airbnb-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-schedule-schema.json\",\n  \"title\": \"Schedule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the schedule entry.\"\n    },\n    \"experience_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the associated experience.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the scheduled session.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"The start time in HH:MM format.\",\n      \"pattern\": \"^[0-2][0-9]:[0-5][0-9]$\"\n    },\n    \"end_time\": {\n      \"type\": \"string\",\n      \"description\": \"The end time in HH:MM format.\",\n      \"pattern\": \"^[0-2][0-9]:[0-5][0-9]$\"\
  \n    },\n    \"max_guests\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of guests for this session.\",\n      \"minimum\": 1\n    },\n    \"booked_guests\": {\n      \"type\": \"integer\",\n      \"description\": \"The current number of booked guests.\",\n      \"minimum\": 0\n    },\n    \"available_spots\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of remaining available spots.\",\n      \"minimum\": 0\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the schedule entry.\",\n      \"enum\": [\n        \"open\",\n        \"full\",\n        \"cancelled\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-schedule-schema.json
tags: []
title: Schedule
---
