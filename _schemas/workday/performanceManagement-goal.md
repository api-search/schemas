---
description: ''
layout: schema
name: Goal
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: The status of the goal (e.g., Not Started, In Progress, Completed).
  name: status
  type: string
- description: ''
  name: dueDate
  type: string
- description: ''
  name: completionDate
  type: string
- description: ''
  name: weight
  type: number
provider_name: Workday
provider_slug: workday
schema_file: json-schema/performanceManagement-goal-schema.json
slug: performanceManagement-goal
source_filename: performanceManagement-goal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Goal\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the goal (e.g., Not Started, In Progress, Completed).\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\"\n    },\n    \"completionDate\": {\n      \"type\": \"string\"\n    },\n    \"weight\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/performanceManagement-goal-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Goal
---
