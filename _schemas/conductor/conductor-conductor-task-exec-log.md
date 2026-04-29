---
description: ''
layout: schema
name: TaskExecLog
properties_list:
- description: Log message
  name: log
  type: string
- description: Associated task ID
  name: taskId
  type: string
- description: Timestamp of the log entry
  name: createdTime
  type: integer
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-task-exec-log-schema.json
slug: conductor-conductor-task-exec-log
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskExecLog\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"log\": {\n      \"type\": \"string\",\n      \"description\": \"Log message\"\n    },\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated task ID\"\n    },\n    \"createdTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp of the log entry\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-task-exec-log-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: TaskExecLog
---
