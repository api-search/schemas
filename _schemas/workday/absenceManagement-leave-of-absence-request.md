---
description: ''
layout: schema
name: LeaveOfAbsenceRequest
properties_list:
- description: ''
  name: firstDayOfLeave
  type: string
- description: ''
  name: estimatedLastDayOfLeave
  type: string
- description: ''
  name: lastDayOfWork
  type: string
- description: ''
  name: firstDayBackAtWork
  type: string
- description: ''
  name: comment
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/absenceManagement-leave-of-absence-request-schema.json
slug: absenceManagement-leave-of-absence-request
source_filename: absenceManagement-leave-of-absence-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LeaveOfAbsenceRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstDayOfLeave\": {\n      \"type\": \"string\"\n    },\n    \"estimatedLastDayOfLeave\": {\n      \"type\": \"string\"\n    },\n    \"lastDayOfWork\": {\n      \"type\": \"string\"\n    },\n    \"firstDayBackAtWork\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/absenceManagement-leave-of-absence-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: LeaveOfAbsenceRequest
---
