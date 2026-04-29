---
description: ''
layout: schema
name: ScheduledJob
properties_list:
- description: ''
  name: id
  type: string
- description: The job category
  name: category
  type: string
- description: The job status
  name: status
  type: string
- description: The job description
  name: description
  type: string
- description: Error message if the job failed
  name: errorMessage
  type: string
- description: ''
  name: startDateTime
  type: string
- description: ''
  name: endDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-scheduled-job-schema.json
slug: automation-scheduled-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScheduledJob\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The job category\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The job status\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The job description\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the job failed\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-scheduled-job-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: ScheduledJob
---
