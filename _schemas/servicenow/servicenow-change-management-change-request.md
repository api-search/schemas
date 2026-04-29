---
description: A ServiceNow change request record.
layout: schema
name: ChangeRequest
properties_list:
- description: Unique identifier for the change request.
  name: sys_id
  type: string
- description: The human-readable change request number.
  name: number
  type: string
- description: A brief summary of the change.
  name: short_description
  type: string
- description: A detailed description of the change and its purpose.
  name: description
  type: string
- description: 'The change type: normal, standard, or emergency.'
  name: type
  type: string
- description: The current state of the change request in its lifecycle.
  name: state
  type: string
- description: The priority level of the change request.
  name: priority
  type: string
- description: The risk level assessed for this change.
  name: risk
  type: string
- description: The impact level of this change.
  name: impact
  type: string
- description: The category of the change.
  name: category
  type: string
- description: The sys_id of the user assigned to implement the change.
  name: assigned_to
  type: string
- description: The sys_id of the group responsible for the change.
  name: assignment_group
  type: string
- description: The sys_id of the user who requested the change.
  name: requested_by
  type: string
- description: The planned start date and time for the change.
  name: start_date
  type: string
- description: The planned end date and time for the change.
  name: end_date
  type: string
- description: The sys_id of the configuration item affected by this change.
  name: cmdb_ci
  type: string
- description: The close code indicating how the change was resolved.
  name: close_code
  type: string
- description: Notes recorded when closing the change request.
  name: close_notes
  type: string
- description: The current approval status.
  name: approval
  type: string
- description: The date and time the change request was created.
  name: sys_created_on
  type: string
- description: The date and time the change request was last updated.
  name: sys_updated_on
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-change-management-change-request-schema.json
slug: servicenow-change-management-change-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A ServiceNow change request record.\",\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the change request.\",\n      \"example\": \"500123\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable change request number.\",\n      \"example\": \"example_value\"\n    },\n    \"short_description\": {\n      \"type\": \"string\",\n      \"description\": \"A brief summary of the change.\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the change and its purpose.\",\n      \"example\": \"A sample description.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The change type: normal, standard, or emergency.\",\n      \"example\": \"normal\",\n      \"enum\": [\n        \"normal\",\n   \
  \     \"standard\",\n        \"emergency\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the change request in its lifecycle.\",\n      \"example\": \"example_value\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"The priority level of the change request.\",\n      \"example\": \"1\",\n      \"enum\": [\n        \"1\",\n        \"2\",\n        \"3\",\n        \"4\"\n      ]\n    },\n    \"risk\": {\n      \"type\": \"string\",\n      \"description\": \"The risk level assessed for this change.\",\n      \"example\": \"example_value\"\n    },\n    \"impact\": {\n      \"type\": \"string\",\n      \"description\": \"The impact level of this change.\",\n      \"example\": \"example_value\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the change.\",\n      \"example\": \"example_value\"\n    },\n    \"assigned_to\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The sys_id of the user assigned to implement the change.\",\n      \"example\": \"example_value\"\n    },\n    \"assignment_group\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the group responsible for the change.\",\n      \"example\": \"example_value\"\n    },\n    \"requested_by\": {\n      \"type\": \"string\",\n      \"description\": \"The sys_id of the user who requested the change.\",\n      \"example\": \"example_value\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"description\": \"The planned start date and time for the change.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"description\": \"The planned end date and time for the change.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"cmdb_ci\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The sys_id of the configuration item affected by this change.\",\n      \"example\": \"example_value\"\n    },\n    \"close_code\": {\n      \"type\": \"string\",\n      \"description\": \"The close code indicating how the change was resolved.\",\n      \"example\": \"example_value\"\n    },\n    \"close_notes\": {\n      \"type\": \"string\",\n      \"description\": \"Notes recorded when closing the change request.\",\n      \"example\": \"example_value\"\n    },\n    \"approval\": {\n      \"type\": \"string\",\n      \"description\": \"The current approval status.\",\n      \"example\": \"example_value\"\n    },\n    \"sys_created_on\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the change request was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"sys_updated_on\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the change request was last updated.\",\n      \"format\"\
  : \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChangeRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-change-management-change-request-schema.json
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
title: ChangeRequest
---
