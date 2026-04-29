---
description: A top-level Acronis backup or protection task
layout: schema
name: Task
properties_list:
- description: Task unique identifier
  name: id
  type: string
- description: Task UUID
  name: uuid
  type: string
- description: Task type (backup, restore, replication, etc.)
  name: type
  type: string
- description: Current task state
  name: state
  type: string
- description: Task result upon completion
  name: result_code
  type: string
- description: Task execution priority
  name: priority
  type: string
- description: Protection policy that initiated this task
  name: policy_id
  type: string
- description: Protected resource this task operates on
  name: resource_id
  type: string
- description: Agent or executor that ran the task
  name: executor_id
  type: string
- description: When the task was queued
  name: enqueuedAt
  type: string
- description: When task execution began
  name: startedAt
  type: string
- description: When task completed
  name: completedAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: tenant_id
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/task-manager-task-schema.json
slug: task-manager-task
source_filename: task-manager-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/task-manager-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"A top-level Acronis backup or protection task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Task unique identifier\",\n      \"example\": \"task-uuid-001\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Task UUID\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Task type (backup, restore, replication, etc.)\",\n      \"example\": \"backup\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"enqueued\",\n        \"assigned\",\n        \"started\",\n        \"paused\",\n        \"completed\"\n      ],\n      \"description\": \"Current task\
  \ state\",\n      \"example\": \"completed\"\n    },\n    \"result_code\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ok\",\n        \"error\",\n        \"warning\",\n        \"cancelled\",\n        \"abandoned\",\n        \"timedout\"\n      ],\n      \"description\": \"Task result upon completion\",\n      \"example\": \"ok\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Task execution priority\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Protection policy that initiated this task\"\n    },\n    \"resource_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Protected resource this task operates on\"\n    },\n    \"executor_id\": {\n      \"type\": \"string\",\n      \"description\": \"Agent or executor that ran the task\"\n    },\n    \"enqueuedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n   \
  \   \"description\": \"When the task was queued\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When task execution began\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When task completed\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/task-manager-task-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: Task
---
