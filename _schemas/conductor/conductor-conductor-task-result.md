---
description: ''
layout: schema
name: TaskResult
properties_list:
- description: The workflow instance ID
  name: workflowInstanceId
  type: string
- description: The task ID
  name: taskId
  type: string
- description: Task execution status
  name: status
  type: string
- description: Task output data
  name: outputData
  type: object
- description: Reason for failure
  name: reasonForIncompletion
  type: string
- description: Callback delay for IN_PROGRESS tasks
  name: callbackAfterSeconds
  type: integer
- description: ID of the worker updating the task
  name: workerId
  type: string
- description: Task execution logs
  name: logs
  type: array
- description: Path to externally stored output payload
  name: externalOutputPayloadStoragePath
  type: string
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-task-result-schema.json
slug: conductor-conductor-task-result
source_filename: conductor-conductor-task-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TaskResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workflowInstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The workflow instance ID\"\n    },\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"The task ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Task execution status\"\n    },\n    \"outputData\": {\n      \"type\": \"object\",\n      \"description\": \"Task output data\"\n    },\n    \"reasonForIncompletion\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for failure\"\n    },\n    \"callbackAfterSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Callback delay for IN_PROGRESS tasks\"\n    },\n    \"workerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the worker updating the task\"\n    },\n    \"logs\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Task execution logs\"\n    },\n    \"externalOutputPayloadStoragePath\": {\n      \"type\": \"string\",\n      \"description\": \"Path to externally stored output payload\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-task-result-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: TaskResult
---
