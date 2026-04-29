---
description: Task schema from Oracle Integration Process Automation API.
layout: schema
name: Task
properties_list:
- description: Task identifier.
  name: id
  type: string
- description: Task title.
  name: title
  type: string
- description: Current assignee.
  name: assignee
  type: string
- description: Task state.
  name: state
  type: string
- description: Task priority.
  name: priority
  type: integer
- description: Task creation timestamp.
  name: createdDate
  type: string
- description: Task due date.
  name: dueDate
  type: string
- description: Parent process instance identifier.
  name: processId
  type: string
- description: Parent process name.
  name: processName
  type: string
- description: Task outcome.
  name: outcome
  type: string
provider_name: Oracle Integration
provider_slug: oracle-integration
schema_file: json-schema/process-automation-api-task-schema.json
slug: process-automation-api-task
source_filename: process-automation-api-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/process-automation-api-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"Task schema from Oracle Integration Process Automation API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\"type\": \"string\", \"description\": \"Task identifier.\"},\n    \"title\": {\"type\": \"string\", \"description\": \"Task title.\"},\n    \"assignee\": {\"type\": \"string\", \"description\": \"Current assignee.\"},\n    \"state\": {\"type\": \"string\", \"description\": \"Task state.\", \"enum\": [\"ASSIGNED\", \"COMPLETED\", \"EXPIRED\", \"INFO_REQUESTED\", \"SUSPENDED\", \"WITHDRAWN\"]},\n    \"priority\": {\"type\": \"integer\", \"description\": \"Task priority.\"},\n    \"createdDate\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Task creation timestamp.\"},\n\
  \    \"dueDate\": {\"type\": \"string\", \"format\": \"date-time\", \"description\": \"Task due date.\"},\n    \"processId\": {\"type\": \"string\", \"description\": \"Parent process instance identifier.\"},\n    \"processName\": {\"type\": \"string\", \"description\": \"Parent process name.\"},\n    \"outcome\": {\"type\": \"string\", \"description\": \"Task outcome.\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/json-schema/process-automation-api-task-schema.json
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
title: Task
---
