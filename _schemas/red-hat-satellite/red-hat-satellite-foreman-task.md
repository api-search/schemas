---
description: An asynchronous task object returned for long-running operations such as publishing content views or uploading manifests.
layout: schema
name: ForemanTask
properties_list:
- description: Unique task identifier.
  name: id
  type: string
- description: Machine-readable task label.
  name: label
  type: string
- description: Whether the task is still pending.
  name: pending
  type: boolean
- description: Human-readable description of the task action.
  name: action
  type: string
- description: User who initiated the task.
  name: username
  type: string
- description: Current state of the task.
  name: state
  type: string
- description: Result of the task.
  name: result
  type: string
- description: Task progress as a decimal (0.0 to 1.0).
  name: progress
  type: number
- description: ''
  name: started_at
  type: '[''string'', ''null'']'
- description: ''
  name: ended_at
  type: '[''string'', ''null'']'
- description: ''
  name: humanized
  type: object
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-foreman-task-schema.json
slug: red-hat-satellite-foreman-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ForemanTask\",\n  \"type\": \"object\",\n  \"description\": \"An asynchronous task object returned for long-running operations such as publishing content views or uploading manifests.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique task identifier.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable task label.\"\n    },\n    \"pending\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the task is still pending.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the task action.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"User who initiated the task.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the task.\"\n    },\n \
  \   \"result\": {\n      \"type\": \"string\",\n      \"description\": \"Result of the task.\"\n    },\n    \"progress\": {\n      \"type\": \"number\",\n      \"description\": \"Task progress as a decimal (0.0 to 1.0).\"\n    },\n    \"started_at\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"ended_at\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"humanized\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-foreman-task-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: ForemanTask
---
