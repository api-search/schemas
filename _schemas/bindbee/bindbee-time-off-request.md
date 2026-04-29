---
description: An employee time-off request from a connected HRIS system.
layout: schema
name: TimeOffRequest
properties_list:
- description: Time-off request ID.
  name: id
  type: string
- description: Employee ID.
  name: employee_id
  type: string
- description: Type of time off.
  name: type
  type: string
- description: Approval status.
  name: status
  type: string
- description: Time-off start date.
  name: start_date
  type: string
- description: Time-off end date.
  name: end_date
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-time-off-request-schema.json
slug: bindbee-time-off-request
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TimeOffRequest\",\n  \"type\": \"object\",\n  \"description\": \"An employee time-off request from a connected HRIS system.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Time-off request ID.\",\n      \"example\": \"to-abc123\"\n    },\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employee ID.\",\n      \"example\": \"emp-abc123\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of time off.\",\n      \"enum\": [\n        \"vacation\",\n        \"sick\",\n        \"personal\",\n        \"other\"\n      ],\n      \"example\": \"vacation\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Approval status.\",\n      \"enum\": [\n        \"pending\",\n        \"approved\",\n        \"rejected\"\n      ],\n      \"example\": \"approved\"\n    },\n    \"start_date\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Time-off start date.\",\n      \"example\": \"2024-07-01\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Time-off end date.\",\n      \"example\": \"2024-07-05\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-time-off-request-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: TimeOffRequest
---
