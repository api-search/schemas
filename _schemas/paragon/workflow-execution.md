---
description: A Workflow Execution represents a single historical run of an integration workflow, including its status, duration, and task count.
layout: schema
name: Paragon Workflow Execution
properties_list:
- description: The unique identifier for the workflow execution.
  name: id
  type: string
- description: The Connected User ID associated with this execution.
  name: userId
  type: string
- description: The workflow ID that was executed.
  name: workflowId
  type: string
- description: The status of the workflow execution.
  name: status
  type: string
- description: The number of tasks executed in this workflow run.
  name: taskCount
  type: integer
- description: The duration of the workflow execution in milliseconds.
  name: runDuration
  type: integer
- description: The date and time the workflow execution started (ISO 8601).
  name: dateStarted
  type: string
- description: The date and time the workflow execution ended (ISO 8601).
  name: dateEnded
  type: string
provider_name: Paragon
provider_slug: paragon
schema_file: json-schema/workflow-execution.json
slug: workflow-execution
source_filename: workflow-execution.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/paragon/blob/main/json-schema/workflow-execution.json\",\n  \"title\": \"Paragon Workflow Execution\",\n  \"description\": \"A Workflow Execution represents a single historical run of an integration workflow, including its status, duration, and task count.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the workflow execution.\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"The Connected User ID associated with this execution.\"\n    },\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"The workflow ID that was executed.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the workflow execution.\",\n      \"enum\": [\"SUCCEEDED\", \"FAILED\"]\n    },\n    \"\
  taskCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of tasks executed in this workflow run.\"\n    },\n    \"runDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"The duration of the workflow execution in milliseconds.\"\n    },\n    \"dateStarted\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the workflow execution started (ISO 8601).\"\n    },\n    \"dateEnded\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the workflow execution ended (ISO 8601).\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/json-schema/workflow-execution.json
tags:
- Embedded iPaaS
- Integrations
title: Paragon Workflow Execution
---
