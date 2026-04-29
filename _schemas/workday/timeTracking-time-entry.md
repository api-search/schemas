---
description: ''
layout: schema
name: TimeEntry
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: date
  type: string
- description: The number of hours entered.
  name: hours
  type: number
- description: ''
  name: comment
  type: string
- description: ''
  name: status
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/timeTracking-time-entry-schema.json
slug: timeTracking-time-entry
source_filename: timeTracking-time-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"date\": {\n      \"type\": \"string\"\n    },\n    \"hours\": {\n      \"type\": \"number\",\n      \"description\": \"The number of hours entered.\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/timeTracking-time-entry-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TimeEntry
---
