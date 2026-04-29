---
description: ''
layout: schema
name: TaskSummary
properties_list:
- description: ''
  name: taskId
  type: string
- description: ''
  name: taskType
  type: string
- description: ''
  name: taskDefName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: workflowId
  type: string
- description: ''
  name: workflowType
  type: string
- description: ''
  name: correlationId
  type: string
- description: ''
  name: scheduledTime
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: updateTime
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: input
  type: string
- description: ''
  name: output
  type: string
- description: ''
  name: reasonForIncompletion
  type: string
- description: ''
  name: queueWaitTime
  type: integer
- description: ''
  name: domain
  type: string
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-task-summary-schema.json
slug: conductor-conductor-task-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\"\n    },\n    \"taskType\": {\n      \"type\": \"string\"\n    },\n    \"taskDefName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"workflowId\": {\n      \"type\": \"string\"\n    },\n    \"workflowType\": {\n      \"type\": \"string\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\"\n    },\n    \"scheduledTime\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\"\n    },\n    \"endTime\": {\n      \"type\": \"string\"\n    },\n    \"input\": {\n      \"type\": \"string\"\n    },\n    \"output\": {\n      \"type\": \"string\"\n    },\n    \"reasonForIncompletion\": {\n      \"type\": \"string\"\n    },\n    \"queueWaitTime\"\
  : {\n      \"type\": \"integer\"\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-task-summary-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: TaskSummary
---
