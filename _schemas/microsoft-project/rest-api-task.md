---
description: Task schema from Microsoft Project Online REST API
layout: schema
name: Task
properties_list:
- description: Unique identifier of the task
  name: Id
  type: string
- description: Name of the task
  name: Name
  type: string
- description: Task start date
  name: Start
  type: string
- description: Task finish date
  name: Finish
  type: string
- description: Task duration in days
  name: Duration
  type: string
- description: Task completion percentage
  name: PercentComplete
  type: integer
- description: Whether this is a summary task
  name: IsSummary
  type: boolean
- description: Whether this is a milestone
  name: IsMilestone
  type: boolean
- description: Task priority (0-1000)
  name: Priority
  type: integer
- description: Parent task ID for subtasks
  name: ParentId
  type: string
- description: Task notes
  name: Notes
  type: string
- description: Whether the task is manually scheduled
  name: IsManuallyScheduled
  type: boolean
- description: Scheduling constraint type
  name: ConstraintType
  type: integer
- description: Constraint date
  name: ConstraintStartEnd
  type: string
- description: Total scheduled work
  name: Work
  type: string
- description: Remaining work
  name: RemainingWork
  type: string
- description: Actual work completed
  name: ActualWork
  type: string
- description: Total cost
  name: Cost
  type: number
provider_name: Microsoft Project
provider_slug: microsoft-project
schema_file: json-schema/rest-api-task-schema.json
slug: rest-api-task
source_filename: rest-api-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"Task schema from Microsoft Project Online REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of the task\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the task\"\n    },\n    \"Start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Task start date\"\n    },\n    \"Finish\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Task finish date\"\n    },\n    \"Duration\": {\n      \"type\": \"string\",\n      \"description\": \"Task duration in days\"\n    },\n    \"PercentComplete\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Task completion percentage\"\n    },\n    \"IsSummary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a summary task\"\n    },\n    \"IsMilestone\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a milestone\"\n    },\n    \"Priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Task priority (0-1000)\"\n    },\n    \"ParentId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Parent task ID for subtasks\"\n    },\n    \"Notes\": {\n      \"type\": \"string\",\n      \"description\": \"Task notes\"\n    },\n    \"IsManuallyScheduled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the task is manually scheduled\"\n    },\n    \"ConstraintType\": {\n      \"type\": \"integer\",\n      \"description\": \"Scheduling constraint type\"\n    },\n    \"ConstraintStartEnd\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"date-time\",\n      \"description\": \"Constraint date\"\n    },\n    \"Work\": {\n      \"type\": \"string\",\n      \"description\": \"Total scheduled work\"\n    },\n    \"RemainingWork\": {\n      \"type\": \"string\",\n      \"description\": \"Remaining work\"\n    },\n    \"ActualWork\": {\n      \"type\": \"string\",\n      \"description\": \"Actual work completed\"\n    },\n    \"Cost\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total cost\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-task-schema.json
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
title: Task
---
