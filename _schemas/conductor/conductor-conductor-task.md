---
description: ''
layout: schema
name: Task
properties_list:
- description: Unique task instance ID
  name: taskId
  type: string
- description: The type of the task
  name: taskType
  type: string
- description: Current status of the task
  name: status
  type: string
- description: Reference name of the task in the workflow
  name: referenceTaskName
  type: string
- description: ID of the workflow instance this task belongs to
  name: workflowInstanceId
  type: string
- description: Type/name of the workflow
  name: workflowType
  type: string
- description: Correlation ID
  name: correlationId
  type: string
- description: Scheduled time
  name: scheduledTime
  type: integer
- description: Start time
  name: startTime
  type: integer
- description: End time
  name: endTime
  type: integer
- description: Last update time
  name: updateTime
  type: integer
- description: Current retry count
  name: retryCount
  type: integer
- description: Number of times this task was polled
  name: pollCount
  type: integer
- description: Callback delay in seconds
  name: callbackAfterSeconds
  type: integer
- description: ID of the worker that polled this task
  name: workerId
  type: string
- description: Task input data
  name: inputData
  type: object
- description: Task output data
  name: outputData
  type: object
- description: Reason for failure
  name: reasonForIncompletion
  type: string
- description: Task execution logs
  name: logs
  type: array
- description: Task domain
  name: domain
  type: string
- description: Sequence number
  name: seq
  type: integer
- description: Task definition name
  name: taskDefName
  type: string
- description: Response timeout
  name: responseTimeoutSeconds
  type: integer
- description: Time spent waiting in queue
  name: queueWaitTime
  type: integer
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-task-schema.json
slug: conductor-conductor-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique task instance ID\"\n    },\n    \"taskType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the task\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the task\"\n    },\n    \"referenceTaskName\": {\n      \"type\": \"string\",\n      \"description\": \"Reference name of the task in the workflow\"\n    },\n    \"workflowInstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the workflow instance this task belongs to\"\n    },\n    \"workflowType\": {\n      \"type\": \"string\",\n      \"description\": \"Type/name of the workflow\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation ID\"\n    },\n    \"scheduledTime\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Scheduled time\"\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Start time\"\n    },\n    \"endTime\": {\n      \"type\": \"integer\",\n      \"description\": \"End time\"\n    },\n    \"updateTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last update time\"\n    },\n    \"retryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Current retry count\"\n    },\n    \"pollCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times this task was polled\"\n    },\n    \"callbackAfterSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Callback delay in seconds\"\n    },\n    \"workerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the worker that polled this task\"\n    },\n    \"inputData\": {\n      \"type\": \"object\",\n      \"description\": \"Task input data\"\n    },\n    \"outputData\": {\n   \
  \   \"type\": \"object\",\n      \"description\": \"Task output data\"\n    },\n    \"reasonForIncompletion\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for failure\"\n    },\n    \"logs\": {\n      \"type\": \"array\",\n      \"description\": \"Task execution logs\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Task domain\"\n    },\n    \"seq\": {\n      \"type\": \"integer\",\n      \"description\": \"Sequence number\"\n    },\n    \"taskDefName\": {\n      \"type\": \"string\",\n      \"description\": \"Task definition name\"\n    },\n    \"responseTimeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Response timeout\"\n    },\n    \"queueWaitTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Time spent waiting in queue\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-task-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: Task
---
