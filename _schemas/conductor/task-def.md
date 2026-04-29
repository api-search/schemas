---
description: A Conductor task definition that specifies the behavior, retry logic, timeout policies, rate limiting, and ownership for a reusable task type.
layout: schema
name: TaskDef
properties_list:
- description: The name of the task definition
  name: name
  type: string
- description: Description of the task
  name: description
  type: string
- description: Number of retries
  name: retryCount
  type: integer
- description: Retry logic
  name: retryLogic
  type: string
- description: Delay between retries in seconds
  name: retryDelaySeconds
  type: integer
- description: Task execution timeout in seconds
  name: timeoutSeconds
  type: integer
- description: Timeout policy
  name: timeoutPolicy
  type: string
- description: Time to wait for worker to respond after polling
  name: responseTimeoutSeconds
  type: integer
- description: Time to wait when polling for task
  name: pollTimeoutSeconds
  type: integer
- description: Concurrent execution limit for the task
  name: concurrentExecLimit
  type: integer
- description: Rate limit per frequency
  name: rateLimitPerFrequency
  type: integer
- description: Rate limit frequency window in seconds
  name: rateLimitFrequencyInSeconds
  type: integer
- description: Email of the task definition owner
  name: ownerEmail
  type: string
- description: Expected input keys
  name: inputKeys
  type: array
- description: Expected output keys
  name: outputKeys
  type: array
- description: Default input template
  name: inputTemplate
  type: object
- description: Creator of the task definition
  name: createdBy
  type: string
- description: Creation timestamp in epoch milliseconds
  name: createTime
  type: integer
- description: Last updater
  name: updatedBy
  type: string
- description: Last update timestamp in epoch milliseconds
  name: updateTime
  type: integer
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/task-def.json
slug: task-def
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/task-def.json\",\n  \"title\": \"TaskDef\",\n  \"description\": \"A Conductor task definition that specifies the behavior, retry logic, timeout policies, rate limiting, and ownership for a reusable task type.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the task definition\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the task\"\n    },\n    \"retryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of retries\",\n      \"default\": 3\n    },\n    \"retryLogic\": {\n      \"type\": \"string\",\n      \"description\": \"Retry logic\",\n      \"enum\": [\n        \"FIXED\",\n        \"EXPONENTIAL_BACKOFF\"\
  ,\n        \"LINEAR_BACKOFF\"\n      ]\n    },\n    \"retryDelaySeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Delay between retries in seconds\",\n      \"default\": 60\n    },\n    \"timeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Task execution timeout in seconds\",\n      \"default\": 0\n    },\n    \"timeoutPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Timeout policy\",\n      \"enum\": [\n        \"RETRY\",\n        \"TIME_OUT_WF\",\n        \"ALERT_ONLY\"\n      ]\n    },\n    \"responseTimeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to wait for worker to respond after polling\",\n      \"default\": 3600\n    },\n    \"pollTimeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to wait when polling for task\"\n    },\n    \"concurrentExecLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Concurrent execution limit for the task\"\n    },\n\
  \    \"rateLimitPerFrequency\": {\n      \"type\": \"integer\",\n      \"description\": \"Rate limit per frequency\"\n    },\n    \"rateLimitFrequencyInSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Rate limit frequency window in seconds\"\n    },\n    \"ownerEmail\": {\n      \"type\": \"string\",\n      \"description\": \"Email of the task definition owner\",\n      \"format\": \"email\"\n    },\n    \"inputKeys\": {\n      \"type\": \"array\",\n      \"description\": \"Expected input keys\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"outputKeys\": {\n      \"type\": \"array\",\n      \"description\": \"Expected output keys\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"inputTemplate\": {\n      \"type\": \"object\",\n      \"description\": \"Default input template\",\n      \"additionalProperties\": true\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Creator of the\
  \ task definition\"\n    },\n    \"createTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation timestamp in epoch milliseconds\"\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Last updater\"\n    },\n    \"updateTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last update timestamp in epoch milliseconds\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/task-def.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: TaskDef
---
