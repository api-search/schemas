---
description: A Task represents an asynchronous operation in VMware Cloud Foundation that tracks the progress and status of long-running infrastructure management activities.
layout: schema
name: Broadcom Task
properties_list:
- description: The unique identifier of the task.
  name: id
  type: string
- description: The name of the task.
  name: name
  type: string
- description: The type of the task operation.
  name: type
  type: string
- description: The current status of the task.
  name: status
  type: string
- description: The timestamp when the task was created.
  name: creationTimestamp
  type: string
- description: The timestamp when the task completed.
  name: completionTimestamp
  type: string
- description: Whether the task can be cancelled.
  name: isCancellable
  type: boolean
- description: Whether the task can be retried after failure.
  name: isRetryable
  type: boolean
- description: The resources associated with this task.
  name: resources
  type: array
- description: The subtasks that make up this task.
  name: subTasks
  type: array
- description: Errors encountered during task execution.
  name: errors
  type: array
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-task-schema.json
slug: broadcom-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/broadcom/blob/main/json-schema/broadcom-task-schema.json\",\n  \"title\": \"Broadcom Task\",\n  \"description\": \"A Task represents an asynchronous operation in VMware Cloud Foundation that tracks the progress and status of long-running infrastructure management activities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the task.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the task.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the task operation.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IN_PROGRESS\",\n        \"SUCCESSFUL\",\n        \"FAILED\",\n        \"CANCELLED\"\n      ],\n      \"description\": \"The current status\
  \ of the task.\"\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the task was created.\"\n    },\n    \"completionTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the task completed.\"\n    },\n    \"isCancellable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the task can be cancelled.\"\n    },\n    \"isRetryable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the task can be retried after failure.\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"resourceId\": {\n            \"type\": \"string\",\n            \"description\": \"The identifier of the associated resource.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\":\
  \ \"The type of the associated resource.\"\n          }\n        }\n      },\n      \"description\": \"The resources associated with this task.\"\n    },\n    \"subTasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the subtask.\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"IN_PROGRESS\",\n              \"SUCCESSFUL\",\n              \"FAILED\",\n              \"CANCELLED\",\n              \"PENDING\"\n            ],\n            \"description\": \"The current status of the subtask.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of the subtask.\"\n          }\n        }\n      },\n      \"description\": \"The subtasks that make up this task.\"\n    },\n    \"errors\": {\n\
  \      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"errorCode\": {\n            \"type\": \"string\",\n            \"description\": \"The error code.\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"The error message.\"\n          },\n          \"remediationMessage\": {\n            \"type\": \"string\",\n            \"description\": \"Guidance on how to resolve the error.\"\n          }\n        }\n      },\n      \"description\": \"Errors encountered during task execution.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/json-schema/broadcom-task-schema.json
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Task
---
