---
description: TimeSheet schema from Microsoft Project Online REST API
layout: schema
name: TimeSheet
properties_list:
- description: Timesheet identifier
  name: Id
  type: string
- description: Timesheet status (0=InProgress, 1=Submitted, 2=Acceptable, 3=Approved, 4=Rejected)
  name: Status
  type: integer
- description: Associated period ID
  name: PeriodId
  type: string
- description: Total work reported
  name: TotalWork
  type: string
- description: Total actual work
  name: TotalActualWork
  type: string
provider_name: Microsoft Project
provider_slug: microsoft-project
schema_file: json-schema/rest-api-time-sheet-schema.json
slug: rest-api-time-sheet
source_filename: rest-api-time-sheet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-time-sheet-schema.json\",\n  \"title\": \"TimeSheet\",\n  \"description\": \"TimeSheet schema from Microsoft Project Online REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Timesheet identifier\"\n    },\n    \"Status\": {\n      \"type\": \"integer\",\n      \"description\": \"Timesheet status (0=InProgress, 1=Submitted, 2=Acceptable, 3=Approved, 4=Rejected)\"\n    },\n    \"PeriodId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Associated period ID\"\n    },\n    \"TotalWork\": {\n      \"type\": \"string\",\n      \"description\": \"Total work reported\"\n    },\n    \"TotalActualWork\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Total actual work\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-time-sheet-schema.json
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
title: TimeSheet
---
