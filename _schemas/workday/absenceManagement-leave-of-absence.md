---
description: ''
layout: schema
name: LeaveOfAbsence
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The start date of the leave.
  name: startDate
  type: string
- description: The estimated end date of the leave.
  name: estimatedEndDate
  type: string
- description: The actual end date of the leave.
  name: actualEndDate
  type: string
- description: The status of the leave (e.g., In Progress, Completed).
  name: status
  type: string
- description: ''
  name: lastDayOfWork
  type: string
- description: ''
  name: firstDayOfWork
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/absenceManagement-leave-of-absence-schema.json
slug: absenceManagement-leave-of-absence
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LeaveOfAbsence\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The start date of the leave.\"\n    },\n    \"estimatedEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"The estimated end date of the leave.\"\n    },\n    \"actualEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"The actual end date of the leave.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the leave (e.g., In Progress, Completed).\"\n    },\n    \"lastDayOfWork\": {\n      \"type\": \"string\"\n    },\n    \"firstDayOfWork\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/absenceManagement-leave-of-absence-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: LeaveOfAbsence
---
