---
description: ''
layout: schema
name: DataChangeTaskCreateRequest
properties_list:
- description: The name for the data change task.
  name: name
  type: string
- description: ''
  name: operation
  type: object
provider_name: Workday
provider_slug: workday
schema_file: json-schema/prismAnalytics-data-change-task-create-request-schema.json
slug: prismAnalytics-data-change-task-create-request
source_filename: prismAnalytics-data-change-task-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataChangeTaskCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the data change task.\"\n    },\n    \"operation\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/prismAnalytics-data-change-task-create-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: DataChangeTaskCreateRequest
---
