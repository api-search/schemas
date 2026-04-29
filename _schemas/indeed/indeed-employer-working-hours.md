---
description: Working hours and schedule information for the position.
layout: schema
name: WorkingHours
properties_list:
- description: Expected number of hours per week.
  name: hoursPerWeek
  type: number
- description: Description of the work schedule.
  name: schedule
  type: string
- description: The type of shift.
  name: shiftType
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-working-hours-schema.json
slug: indeed-employer-working-hours
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkingHours\",\n  \"type\": \"object\",\n  \"description\": \"Working hours and schedule information for the position.\",\n  \"properties\": {\n    \"hoursPerWeek\": {\n      \"type\": \"number\",\n      \"description\": \"Expected number of hours per week.\"\n    },\n    \"schedule\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the work schedule.\"\n    },\n    \"shiftType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of shift.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-working-hours-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: WorkingHours
---
