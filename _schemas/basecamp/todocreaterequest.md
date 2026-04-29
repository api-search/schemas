---
description: ''
layout: schema
name: TodoCreateRequest
properties_list:
- description: To-do text description
  name: content
  type: string
- description: Additional details in HTML format
  name: description
  type: string
- description: Person IDs to assign to this to-do
  name: assignee_ids
  type: array
- description: Person IDs to notify when this to-do is completed
  name: completion_subscriber_ids
  type: array
- description: Whether to immediately notify assignees
  name: notify
  type: boolean
- description: Due date in ISO 8601 format
  name: due_on
  type: string
- description: Start date in ISO 8601 format
  name: starts_on
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/todocreaterequest-schema.json
slug: todocreaterequest
source_filename: todocreaterequest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/todocreaterequest-schema.json\",\n  \"title\": \"TodoCreateRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"content\"\n  ],\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"To-do text description\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details in HTML format\"\n    },\n    \"assignee_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Person IDs to assign to this to-do\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"completion_subscriber_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Person IDs to notify when this to-do is completed\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"notify\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether to immediately notify assignees\"\n    },\n    \"due_on\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Due date in ISO 8601 format\"\n    },\n    \"starts_on\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date in ISO 8601 format\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/todocreaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: TodoCreateRequest
---
