---
description: ''
layout: schema
name: DataChangeTaskActivity
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: activityType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: startedOn
  type: string
- description: ''
  name: completedOn
  type: string
- description: ''
  name: rowsProcessed
  type: integer
- description: ''
  name: rowsFailed
  type: integer
provider_name: Workday
provider_slug: workday
schema_file: json-schema/prismAnalytics-data-change-task-activity-schema.json
slug: prismAnalytics-data-change-task-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataChangeTaskActivity\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"activityType\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"startedOn\": {\n      \"type\": \"string\"\n    },\n    \"completedOn\": {\n      \"type\": \"string\"\n    },\n    \"rowsProcessed\": {\n      \"type\": \"integer\"\n    },\n    \"rowsFailed\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/prismAnalytics-data-change-task-activity-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: DataChangeTaskActivity
---
