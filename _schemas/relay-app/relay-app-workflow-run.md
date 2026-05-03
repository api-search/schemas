---
description: A workflow run instance in Relay.app, representing a single execution of a workflow including its status, timing, and input/output data.
layout: schema
name: Relay App Workflow Run
properties_list:
- description: The unique identifier of the workflow run.
  name: id
  type: string
- description: The ID of the workflow being run.
  name: workflowId
  type: string
- description: Current status of the workflow run.
  name: status
  type: string
- description: Date and time the run was started.
  name: startedAt
  type: string
- description: Date and time the run was completed.
  name: completedAt
  type:
  - string
  - 'null'
- description: Error message if the run failed.
  name: error
  type:
  - string
  - 'null'
- description: Input data provided when the run was triggered.
  name: inputData
  type: object
provider_name: Relay App
provider_slug: relay-app
schema_file: json-schema/relay-app-workflow-run-schema.json
slug: relay-app-workflow-run
source_filename: relay-app-workflow-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/relay-app/main/json-schema/relay-app-workflow-run-schema.json\",\n  \"title\": \"Relay App Workflow Run\",\n  \"description\": \"A workflow run instance in Relay.app, representing a single execution of a workflow including its status, timing, and input/output data.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"workflowId\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the workflow run.\"\n    },\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the workflow being run.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the workflow run.\",\n      \"enum\": [\"running\", \"completed\", \"failed\", \"paused\", \"cancelled\"]\n    },\n    \"startedAt\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the run was started.\"\n    },\n    \"completedAt\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the run was completed.\"\n    },\n    \"error\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Error message if the run failed.\"\n    },\n    \"inputData\": {\n      \"type\": \"object\",\n      \"description\": \"Input data provided when the run was triggered.\",\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/relay-app/refs/heads/main/json-schema/relay-app-workflow-run-schema.json
tags:
- Automation
- Workflow
- Integration
- No-Code
- AI
- Webhooks
title: Relay App Workflow Run
---
