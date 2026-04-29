---
description: Summary representation of a schedule
layout: schema
name: ScheduleSummary
properties_list:
- description: Unique schedule identifier
  name: id
  type: string
- description: Name of the schedule
  name: name
  type: string
- description: ID of the associated workflow
  name: workflowId
  type: string
- description: ID of the schedule owner
  name: ownerId
  type: string
- description: Next scheduled run date and time
  name: runDateTime
  type: string
- description: Time zone for the schedule
  name: timeZone
  type: string
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-schedule-summary-schema.json
slug: alteryx-server-v3-schedule-summary
source_filename: alteryx-server-v3-schedule-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScheduleSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary representation of a schedule\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique schedule identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the schedule\"\n    },\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the associated workflow\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the schedule owner\"\n    },\n    \"runDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Next scheduled run date and time\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone for the schedule\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-schedule-summary-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: ScheduleSummary
---
