---
description: Request body for updating a task
layout: schema
name: PlannerTaskUpdate
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: bucketId
  type: string
- description: ''
  name: priority
  type: integer
- description: ''
  name: percentComplete
  type: integer
- description: ''
  name: startDateTime
  type: string
- description: ''
  name: dueDateTime
  type: string
- description: ''
  name: conversationThreadId
  type: string
- description: ''
  name: orderHint
  type: string
- description: ''
  name: assigneePriority
  type: string
- description: ''
  name: previewType
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-task-update-schema.json
slug: microsoft-planner-planner-task-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerTaskUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a task\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"integer\"\n    },\n    \"percentComplete\": {\n      \"type\": \"integer\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\"\n    },\n    \"dueDateTime\": {\n      \"type\": \"string\"\n    },\n    \"conversationThreadId\": {\n      \"type\": \"string\"\n    },\n    \"orderHint\": {\n      \"type\": \"string\"\n    },\n    \"assigneePriority\": {\n      \"type\": \"string\"\n    },\n    \"previewType\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-task-update-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerTaskUpdate
---
