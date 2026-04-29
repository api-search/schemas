---
description: ''
layout: schema
name: Task
properties_list:
- description: ''
  name: globalId
  type: integer
- description: ''
  name: id
  type: integer
- description: ''
  name: contentId
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: body
  type: string
- description: ''
  name: creator
  type: string
- description: ''
  name: assignee
  type: string
- description: ''
  name: completeUser
  type: string
- description: ''
  name: createDate
  type: integer
- description: ''
  name: dueDate
  type: integer
- description: ''
  name: updateDate
  type: integer
- description: ''
  name: completeDate
  type: integer
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-inline-tasks-task-schema.json
slug: atlassian-confluence-inline-tasks-task
source_filename: atlassian-confluence-inline-tasks-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"globalId\": {\n      \"type\": \"integer\"\n    },\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"contentId\": {\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"body\": {\n      \"type\": \"string\"\n    },\n    \"creator\": {\n      \"type\": \"string\"\n    },\n    \"assignee\": {\n      \"type\": \"string\"\n    },\n    \"completeUser\": {\n      \"type\": \"string\"\n    },\n    \"createDate\": {\n      \"type\": \"integer\"\n    },\n    \"dueDate\": {\n      \"type\": \"integer\"\n    },\n    \"updateDate\": {\n      \"type\": \"integer\"\n    },\n    \"completeDate\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-inline-tasks-task-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Task
---
