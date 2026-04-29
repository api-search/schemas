---
description: Represents the assignment of a task to a user
layout: schema
name: PlannerAssignment
properties_list:
- description: ''
  name: '@odata.type'
  type: string
- description: The time at which the task was assigned
  name: assignedDateTime
  type: string
- description: Hint used to order assignees in a task. The format is defined in the Planner order hints documentation.
  name: orderHint
  type: string
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-assignment-schema.json
slug: microsoft-planner-planner-assignment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerAssignment\",\n  \"type\": \"object\",\n  \"description\": \"Represents the assignment of a task to a user\",\n  \"properties\": {\n    \"@odata.type\": {\n      \"type\": \"string\"\n    },\n    \"assignedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time at which the task was assigned\"\n    },\n    \"orderHint\": {\n      \"type\": \"string\",\n      \"description\": \"Hint used to order assignees in a task. The format is defined in the Planner order hints documentation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-assignment-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerAssignment
---
