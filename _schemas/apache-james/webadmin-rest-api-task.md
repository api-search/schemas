---
description: An asynchronous task
layout: schema
name: Task
properties_list:
- description: Unique task identifier
  name: taskId
  type: string
- description: Task type
  name: type
  type: string
- description: Task status
  name: status
  type: string
- description: When the task was submitted
  name: submitDate
  type: string
- description: When the task started executing
  name: startedDate
  type: string
- description: When the task completed
  name: completedDate
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-task-schema.json
slug: webadmin-rest-api-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"An asynchronous task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique task identifier\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Task type\",\n      \"example\": \"reindexing\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Task status\",\n      \"enum\": [\n        \"waiting\",\n        \"inProgress\",\n        \"completed\",\n        \"failed\",\n        \"cancelled\"\n      ],\n      \"example\": \"completed\"\n    },\n    \"submitDate\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date-time\",\n      \"description\": \"When the task was submitted\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"startedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the task started executing\",\n      \"example\": \"2025-03-15T14:30:01Z\"\n    },\n    \"completedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the task completed\",\n      \"example\": \"2025-03-15T14:30:05Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-task-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: Task
---
