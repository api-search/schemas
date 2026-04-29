---
description: Request body for creating a new schedule.
layout: schema
name: ScheduleCreateRequest
properties_list:
- description: ''
  name: '@type'
  type: string
- description: The name for the new schedule.
  name: name
  type: string
- description: A description of the schedule.
  name: description
  type: string
- description: The scheduled start time.
  name: startTime
  type: string
- description: The scheduled end time.
  name: endTime
  type: string
- description: The recurrence interval.
  name: interval
  type: string
- description: The repeat frequency.
  name: frequency
  type: integer
- description: The time zone.
  name: timezone
  type: string
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-schedule-create-request-schema.json
slug: informatica-platform-rest-schedule-create-request
source_filename: informatica-platform-rest-schedule-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScheduleCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new schedule.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the new schedule.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the schedule.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"The scheduled start time.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"description\": \"The scheduled end time.\"\n    },\n    \"interval\": {\n      \"type\": \"string\",\n      \"description\": \"The recurrence interval.\"\n    },\n    \"frequency\": {\n      \"type\": \"integer\",\n      \"description\": \"The repeat frequency.\"\n    },\n    \"timezone\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The time zone.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-schedule-create-request-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: ScheduleCreateRequest
---
