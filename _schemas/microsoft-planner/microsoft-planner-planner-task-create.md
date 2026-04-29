---
description: Request body for creating a new task
layout: schema
name: PlannerTaskCreate
properties_list:
- description: ID of the plan the task belongs to
  name: planId
  type: string
- description: Title of the task
  name: title
  type: string
- description: ID of the bucket to place the task in
  name: bucketId
  type: string
- description: Priority of the task (0 is highest, 10 is lowest)
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
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-task-create-schema.json
slug: microsoft-planner-planner-task-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerTaskCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new task\",\n  \"properties\": {\n    \"planId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the plan the task belongs to\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the task\"\n    },\n    \"bucketId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the bucket to place the task in\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority of the task (0 is highest, 10 is lowest)\"\n    },\n    \"percentComplete\": {\n      \"type\": \"integer\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\"\n    },\n    \"dueDateTime\": {\n      \"type\": \"string\"\n    },\n    \"conversationThreadId\": {\n      \"type\": \"string\"\n    },\n    \"orderHint\": {\n      \"type\"\
  : \"string\"\n    },\n    \"assigneePriority\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-task-create-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerTaskCreate
---
