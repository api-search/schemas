---
description: ''
layout: schema
name: TimeEntryRequest
properties_list:
- description: ''
  name: date
  type: string
- description: ''
  name: hours
  type: number
- description: ''
  name: comment
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/timeTracking-time-entry-request-schema.json
slug: timeTracking-time-entry-request
source_filename: timeTracking-time-entry-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeEntryRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\"\n    },\n    \"hours\": {\n      \"type\": \"number\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/timeTracking-time-entry-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TimeEntryRequest
---
