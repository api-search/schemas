---
description: A People Task represents a human-in-the-loop task within an Appmixer flow that requires manual approval or action before the workflow can proceed.
layout: schema
name: Appmixer People Task
properties_list:
- description: Unique identifier for the task.
  name: id
  type: string
- description: The flow that generated this task.
  name: flowId
  type: string
- description: The role of the user in relation to this task.
  name: role
  type: string
- description: Current status of the task.
  name: status
  type: string
- description: Timestamp when the task was created.
  name: createdAt
  type: string
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/people-task.json
slug: people-task
source_filename: people-task.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/appmixer/blob/main/json-schema/people-task.json\",\n  \"title\": \"Appmixer People Task\",\n  \"description\": \"A People Task represents a human-in-the-loop task within an Appmixer flow that requires manual approval or action before the workflow can proceed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the task.\"\n    },\n    \"flowId\": {\n      \"type\": \"string\",\n      \"description\": \"The flow that generated this task.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\"approver\", \"requester\"],\n      \"description\": \"The role of the user in relation to this task.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the task.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the task was created.\"\n    }\n  },\n  \"required\": [\"id\", \"flowId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/json-schema/people-task.json
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer People Task
---
