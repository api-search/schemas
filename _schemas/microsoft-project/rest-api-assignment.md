---
description: Assignment schema from Microsoft Project Online REST API
layout: schema
name: Assignment
properties_list:
- description: Assignment identifier
  name: Id
  type: string
- description: Project identifier
  name: ProjectId
  type: string
- description: Task identifier
  name: TaskId
  type: string
- description: Resource identifier
  name: ResourceId
  type: string
- description: Name of the assigned resource
  name: ResourceName
  type: string
- description: Actual work completed
  name: ActualWork
  type: string
- description: Remaining work
  name: RemainingWork
  type: string
- description: Work completion percentage
  name: PercentWorkComplete
  type: integer
- description: Assignment start date
  name: Start
  type: string
- description: Assignment finish date
  name: Finish
  type: string
provider_name: Microsoft Project
provider_slug: microsoft-project
schema_file: json-schema/rest-api-assignment-schema.json
slug: rest-api-assignment
source_filename: rest-api-assignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-assignment-schema.json\",\n  \"title\": \"Assignment\",\n  \"description\": \"Assignment schema from Microsoft Project Online REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Assignment identifier\"\n    },\n    \"ProjectId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Project identifier\"\n    },\n    \"TaskId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Task identifier\"\n    },\n    \"ResourceId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Resource identifier\"\n    },\n    \"ResourceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of\
  \ the assigned resource\"\n    },\n    \"ActualWork\": {\n      \"type\": \"string\",\n      \"description\": \"Actual work completed\"\n    },\n    \"RemainingWork\": {\n      \"type\": \"string\",\n      \"description\": \"Remaining work\"\n    },\n    \"PercentWorkComplete\": {\n      \"type\": \"integer\",\n      \"description\": \"Work completion percentage\"\n    },\n    \"Start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Assignment start date\"\n    },\n    \"Finish\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Assignment finish date\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-assignment-schema.json
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
title: Assignment
---
