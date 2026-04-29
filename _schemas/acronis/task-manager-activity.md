---
description: A subordinate activity within a task
layout: schema
name: Activity
properties_list:
- description: Activity unique identifier
  name: id
  type: string
- description: Activity type
  name: type
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: result_code
  type: string
- description: Parent activity UUID if nested
  name: parent_activity_id
  type: string
- description: Parent task identifier
  name: task_id
  type: string
- description: Whether activity can be requeued on failure
  name: sustainable
  type: boolean
- description: ''
  name: createdAt
  type: string
- description: ''
  name: startedAt
  type: string
- description: ''
  name: completedAt
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/task-manager-activity-schema.json
slug: task-manager-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/task-manager-activity-schema.json\",\n  \"title\": \"Activity\",\n  \"description\": \"A subordinate activity within a task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Activity unique identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Activity type\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"enqueued\",\n        \"assigned\",\n        \"started\",\n        \"paused\",\n        \"completed\"\n      ]\n    },\n    \"result_code\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ok\",\n        \"error\",\n        \"warning\",\n        \"cancelled\",\n        \"abandoned\",\n        \"timedout\"\n      ]\n    },\n    \"parent_activity_id\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Parent activity UUID if nested\"\n    },\n    \"task_id\": {\n      \"type\": \"string\",\n      \"description\": \"Parent task identifier\"\n    },\n    \"sustainable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether activity can be requeued on failure\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"startedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/task-manager-activity-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: Activity
---
