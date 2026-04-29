---
description: A collection of plannerTask resources
layout: schema
name: PlannerTaskCollection
properties_list:
- description: ''
  name: '@odata.context'
  type: string
- description: ''
  name: '@odata.count'
  type: integer
- description: ''
  name: value
  type: array
provider_name: Microsoft Planner
provider_slug: microsoft-planner
schema_file: json-schema/microsoft-planner-planner-task-collection-schema.json
slug: microsoft-planner-planner-task-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlannerTaskCollection\",\n  \"type\": \"object\",\n  \"description\": \"A collection of plannerTask resources\",\n  \"properties\": {\n    \"@odata.context\": {\n      \"type\": \"string\"\n    },\n    \"@odata.count\": {\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-planner/refs/heads/main/json-schema/microsoft-planner-planner-task-collection-schema.json
tags:
- Collaboration
- Microsoft 365
- Productivity
- Project Management
- Task Management
title: PlannerTaskCollection
---
