---
description: Contract for fully updating a schedule (all required fields must be provided)
layout: schema
name: UpdateScheduleContract
properties_list:
- description: ''
  name: workflowId
  type: string
- description: ''
  name: ownerId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: comment
  type: string
- description: ''
  name: priority
  type: string
- description: ''
  name: workerTag
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: credentialId
  type: string
- description: ''
  name: timeZone
  type: string
- description: ''
  name: questions
  type: array
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-update-schedule-contract-schema.json
slug: alteryx-server-v3-update-schedule-contract
source_filename: alteryx-server-v3-update-schedule-contract-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateScheduleContract\",\n  \"type\": \"object\",\n  \"description\": \"Contract for fully updating a schedule (all required fields must be provided)\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"string\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"string\"\n    },\n    \"workerTag\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"credentialId\": {\n      \"type\": \"string\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\"\n    },\n    \"questions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-update-schedule-contract-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: UpdateScheduleContract
---
