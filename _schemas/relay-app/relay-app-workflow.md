---
description: A workflow definition in Relay.app, representing an automated process that can be triggered via webhooks, schedules, app events, or manual activation.
layout: schema
name: Relay App Workflow
properties_list:
- description: The unique identifier of the workflow.
  name: id
  type: string
- description: The name of the workflow.
  name: name
  type: string
- description: Optional description of the workflow.
  name: description
  type: string
- description: Current status of the workflow.
  name: status
  type: string
- description: The type of trigger that starts this workflow.
  name: triggerType
  type: string
- description: Date and time the workflow was created.
  name: createdAt
  type: string
- description: Date and time the workflow was last updated.
  name: updatedAt
  type: string
provider_name: Relay App
provider_slug: relay-app
schema_file: json-schema/relay-app-workflow-schema.json
slug: relay-app-workflow
source_filename: relay-app-workflow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/relay-app/main/json-schema/relay-app-workflow-schema.json\",\n  \"title\": \"Relay App Workflow\",\n  \"description\": \"A workflow definition in Relay.app, representing an automated process that can be triggered via webhooks, schedules, app events, or manual activation.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\", \"triggerType\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the workflow.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the workflow.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of\
  \ the workflow.\",\n      \"enum\": [\"active\", \"inactive\", \"draft\"]\n    },\n    \"triggerType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of trigger that starts this workflow.\",\n      \"enum\": [\"webhook\", \"scheduled\", \"manual\", \"app\", \"form\", \"table\", \"batch\", \"rss\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the workflow was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the workflow was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/relay-app/refs/heads/main/json-schema/relay-app-workflow-schema.json
tags:
- Automation
- Workflow
- Integration
- No-Code
- AI
- Webhooks
title: Relay App Workflow
---
