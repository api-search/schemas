---
description: Contract for creating a new schedule
layout: schema
name: CreateScheduleContract
properties_list:
- description: ID of the workflow to schedule
  name: workflowId
  type: string
- description: Name of the schedule
  name: name
  type: string
- description: Comments about the schedule
  name: comment
  type: string
- description: Execution priority
  name: priority
  type: string
- description: Worker tag for execution routing
  name: workerTag
  type: string
- description: Credential to use for execution
  name: credentialId
  type: string
- description: Time zone for the schedule (defaults to UTC-0)
  name: timeZone
  type: string
- description: Analytic app question values
  name: questions
  type: array
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-create-schedule-contract-schema.json
slug: alteryx-server-v3-create-schedule-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateScheduleContract\",\n  \"type\": \"object\",\n  \"description\": \"Contract for creating a new schedule\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the workflow to schedule\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the schedule\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comments about the schedule\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Execution priority\"\n    },\n    \"workerTag\": {\n      \"type\": \"string\",\n      \"description\": \"Worker tag for execution routing\"\n    },\n    \"credentialId\": {\n      \"type\": \"string\",\n      \"description\": \"Credential to use for execution\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone for\
  \ the schedule (defaults to UTC-0)\"\n    },\n    \"questions\": {\n      \"type\": \"array\",\n      \"description\": \"Analytic app question values\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-create-schedule-contract-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: CreateScheduleContract
---
