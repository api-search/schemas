---
description: ''
layout: schema
name: TimeOffEntry
properties_list:
- description: The Workday ID of the time-off entry.
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The date of the time off.
  name: date
  type: string
- description: The quantity of time off taken.
  name: dailyQuantity
  type: number
- description: The status of the time-off entry.
  name: status
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/absenceManagement-time-off-entry-schema.json
slug: absenceManagement-time-off-entry
source_filename: absenceManagement-time-off-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeOffEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the time-off entry.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the time off.\"\n    },\n    \"dailyQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"The quantity of time off taken.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the time-off entry.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/absenceManagement-time-off-entry-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TimeOffEntry
---
