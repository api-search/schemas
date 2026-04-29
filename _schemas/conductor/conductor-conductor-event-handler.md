---
description: ''
layout: schema
name: EventHandler
properties_list:
- description: Name of the event handler
  name: name
  type: string
- description: Event identifier in the format source:sink:subject (e.g., conductor:workflow_completed:myWorkflow)
  name: event
  type: string
- description: Condition expression to evaluate
  name: condition
  type: string
- description: List of actions to perform when the event is received
  name: actions
  type: array
- description: Whether the event handler is active
  name: active
  type: boolean
- description: Type of evaluator for the condition
  name: evaluatorType
  type: string
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-event-handler-schema.json
slug: conductor-conductor-event-handler
source_filename: conductor-conductor-event-handler-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventHandler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the event handler\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"Event identifier in the format source:sink:subject (e.g., conductor:workflow_completed:myWorkflow)\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"description\": \"Condition expression to evaluate\"\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"description\": \"List of actions to perform when the event is received\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the event handler is active\"\n    },\n    \"evaluatorType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of evaluator for the condition\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-event-handler-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: EventHandler
---
