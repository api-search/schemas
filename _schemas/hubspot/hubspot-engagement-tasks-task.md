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
schema_file: json-schema/hubspot-engagement-tasks-task-schema.json
slug: hubspot-engagement-tasks-task
source_filename: hubspot-engagement-tasks-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A HubSpot task engagement record.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the task.\",\n      \"example\": \"500123\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"The task's properties as key-value pairs.\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"associations\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"Task\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-tasks-task-schema.json
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
