---
description: ''
layout: schema
name: Timesheet
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: periodStartDate
  type: string
- description: ''
  name: periodEndDate
  type: string
- description: ''
  name: totalHours
  type: number
- description: The status of the timesheet (e.g., Draft, Submitted, Approved).
  name: status
  type: string
- description: ''
  name: calculatedEntries
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/timeTracking-timesheet-schema.json
slug: timeTracking-timesheet
source_filename: timeTracking-timesheet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Timesheet\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"periodStartDate\": {\n      \"type\": \"string\"\n    },\n    \"periodEndDate\": {\n      \"type\": \"string\"\n    },\n    \"totalHours\": {\n      \"type\": \"number\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the timesheet (e.g., Draft, Submitted, Approved).\"\n    },\n    \"calculatedEntries\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/timeTracking-timesheet-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Timesheet
---
