---
description: Fields for creating a change task.
layout: schema
name: ChangeTaskInput
properties_list:
- description: A brief summary of the task.
  name: short_description
  type: string
- description: A detailed description of the task.
  name: description
  type: string
- description: The sys_id of the assigned user.
  name: assigned_to
  type: string
- description: The sys_id of the assignment group.
  name: assignment_group
  type: string
- description: The planned start date.
  name: planned_start_date
  type: string
- description: The planned end date.
  name: planned_end_date
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-change-management-change-task-input-schema.json
slug: servicenow-change-management-change-task-input
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Fields for creating a change task.\",\n  \"properties\": {\n    \"short_description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief summary of the task.\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the task.\",\n      \"example\": \"A sample description.\"\n    },\n    \"assigned_to\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the assigned user.\",\n      \"example\": \"example_value\"\n    },\n    \"assignment_group\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the assignment group.\",\n      \"example\": \"example_value\"\n    },\n    \"planned_start_date\": {\n      \"type\": \"string\",\n      \"description\": \"The planned start date.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"planned_end_date\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The planned end date.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChangeTaskInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-change-management-change-task-input-schema.json
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
title: ChangeTaskInput
---
