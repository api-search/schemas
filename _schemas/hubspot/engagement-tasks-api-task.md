---
description: A HubSpot task engagement record.
layout: schema
name: Task
properties_list:
- description: The unique identifier for the task.
  name: id
  type: string
- description: The task's properties as key-value pairs.
  name: properties
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: archived
  type: boolean
- description: ''
  name: associations
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/engagement-tasks-api-task-schema.json
slug: engagement-tasks-api-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-tasks-api-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"A HubSpot task engagement record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the task.\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The task's properties as key-value pairs.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\"\
  : \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"associations\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"results\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/Association\"\n            },\n            \"example\": [\n              {\n                \"id\": \"500123\",\n                \"type\": \"standard\"\n              }\n            ]\n          },\n          \"paging\": {\n            \"$ref\": \"#/components/schemas/Paging\"\n          }\n        }\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/engagement-tasks-api-task-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: Task
---
