---
description: Fields for creating or updating a change request.
layout: schema
name: ChangeRequestInput
properties_list:
- description: A brief summary of the change.
  name: short_description
  type: string
- description: A detailed description of the change.
  name: description
  type: string
- description: The priority level.
  name: priority
  type: string
- description: The risk level.
  name: risk
  type: string
- description: The impact level.
  name: impact
  type: string
- description: The category of the change.
  name: category
  type: string
- description: The sys_id of the assigned user.
  name: assigned_to
  type: string
- description: The sys_id of the assignment group.
  name: assignment_group
  type: string
- description: The sys_id of the requesting user.
  name: requested_by
  type: string
- description: The planned start date and time.
  name: start_date
  type: string
- description: The planned end date and time.
  name: end_date
  type: string
- description: The sys_id of the affected configuration item.
  name: cmdb_ci
  type: string
- description: The business justification for the change.
  name: justification
  type: string
- description: The plan for implementing the change.
  name: implementation_plan
  type: string
- description: The plan for reverting the change if needed.
  name: backout_plan
  type: string
- description: The plan for testing the change.
  name: test_plan
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-change-management-change-request-input-schema.json
slug: servicenow-change-management-change-request-input
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Fields for creating or updating a change request.\",\n  \"properties\": {\n    \"short_description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief summary of the change.\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the change.\",\n      \"example\": \"A sample description.\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"The priority level.\",\n      \"example\": \"1\",\n      \"enum\": [\n        \"1\",\n        \"2\",\n        \"3\",\n        \"4\"\n      ]\n    },\n    \"risk\": {\n      \"type\": \"string\",\n      \"description\": \"The risk level.\",\n      \"example\": \"example_value\"\n    },\n    \"impact\": {\n      \"type\": \"string\",\n      \"description\": \"The impact level.\",\n      \"example\": \"example_value\"\n    },\n    \"category\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The category of the change.\",\n      \"example\": \"example_value\"\n    },\n    \"assigned_to\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the assigned user.\",\n      \"example\": \"example_value\"\n    },\n    \"assignment_group\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the assignment group.\",\n      \"example\": \"example_value\"\n    },\n    \"requested_by\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the requesting user.\",\n      \"example\": \"example_value\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"description\": \"The planned start date and time.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"description\": \"The planned end date and time.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\
  \n    },\n    \"cmdb_ci\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the affected configuration item.\",\n      \"example\": \"example_value\"\n    },\n    \"justification\": {\n      \"type\": \"string\",\n      \"description\": \"The business justification for the change.\",\n      \"example\": \"example_value\"\n    },\n    \"implementation_plan\": {\n      \"type\": \"string\",\n      \"description\": \"The plan for implementing the change.\",\n      \"example\": \"example_value\"\n    },\n    \"backout_plan\": {\n      \"type\": \"string\",\n      \"description\": \"The plan for reverting the change if needed.\",\n      \"example\": \"example_value\"\n    },\n    \"test_plan\": {\n      \"type\": \"string\",\n      \"description\": \"The plan for testing the change.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChangeRequestInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-change-management-change-request-input-schema.json
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
title: ChangeRequestInput
---
