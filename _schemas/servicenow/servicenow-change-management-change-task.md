---
description: A task associated with a change request.
layout: schema
name: ChangeTask
properties_list:
- description: Unique identifier for the change task.
  name: sys_id
  type: string
- description: The human-readable task number.
  name: number
  type: string
- description: A brief summary of the task.
  name: short_description
  type: string
- description: The current state of the task.
  name: state
  type: string
- description: The sys_id of the assigned user.
  name: assigned_to
  type: string
- description: The sys_id of the parent change request.
  name: change_request
  type: string
- description: The planned start date for the task.
  name: planned_start_date
  type: string
- description: The planned end date for the task.
  name: planned_end_date
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-change-management-change-task-schema.json
slug: servicenow-change-management-change-task
source_filename: servicenow-change-management-change-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A task associated with a change request.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the change task.\",\n      \"example\": \"500123\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable task number.\",\n      \"example\": \"example_value\"\n    },\n    \"short_description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief summary of the task.\",\n      \"example\": \"example_value\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the task.\",\n      \"example\": \"example_value\"\n    },\n    \"assigned_to\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the assigned user.\",\n      \"example\": \"example_value\"\n    },\n    \"change_request\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id\
  \ of the parent change request.\",\n      \"example\": \"example_value\"\n    },\n    \"planned_start_date\": {\n      \"type\": \"string\",\n      \"description\": \"The planned start date for the task.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"planned_end_date\": {\n      \"type\": \"string\",\n      \"description\": \"The planned end date for the task.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChangeTask\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-change-management-change-task-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: ChangeTask
---
