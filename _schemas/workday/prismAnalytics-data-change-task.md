---
description: ''
layout: schema
name: DataChangeTask
properties_list:
- description: The Workday ID of the data change task.
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: name
  type: string
- description: The status of the task (e.g., New, Processing, Complete, Error).
  name: status
  type: object
- description: The operation type (e.g., FullReplace, Append).
  name: operation
  type: object
- description: ''
  name: createdOn
  type: string
- description: ''
  name: completedOn
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/prismAnalytics-data-change-task-schema.json
slug: prismAnalytics-data-change-task
source_filename: prismAnalytics-data-change-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataChangeTask\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the data change task.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"The status of the task (e.g., New, Processing, Complete, Error).\"\n    },\n    \"operation\": {\n      \"type\": \"object\",\n      \"description\": \"The operation type (e.g., FullReplace, Append).\"\n    },\n    \"createdOn\": {\n      \"type\": \"string\"\n    },\n    \"completedOn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/prismAnalytics-data-change-task-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: DataChangeTask
---
