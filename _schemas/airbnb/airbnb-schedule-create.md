---
description: ''
layout: schema
name: ScheduleCreate
properties_list:
- description: The date of the scheduled session.
  name: date
  type: string
- description: The start time in HH:MM format.
  name: start_time
  type: string
- description: Override the maximum number of guests for this specific session.
  name: max_guests
  type: integer
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-schedule-create-schema.json
slug: airbnb-schedule-create
source_filename: airbnb-schedule-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-schedule-create-schema.json\",\n  \"title\": \"ScheduleCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the scheduled session.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"The start time in HH:MM format.\",\n      \"pattern\": \"^[0-2][0-9]:[0-5][0-9]$\"\n    },\n    \"max_guests\": {\n      \"type\": \"integer\",\n      \"description\": \"Override the maximum number of guests for this specific session.\",\n      \"minimum\": 1\n    }\n  },\n  \"required\": [\n    \"date\",\n    \"start_time\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-schedule-create-schema.json
tags: []
title: ScheduleCreate
---
