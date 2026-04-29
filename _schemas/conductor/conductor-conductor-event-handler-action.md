---
description: ''
layout: schema
name: EventHandlerAction
properties_list:
- description: The action type
  name: action
  type: string
- description: Start workflow action parameters
  name: start_workflow
  type: object
- description: Complete task action parameters
  name: complete_task
  type: object
- description: Fail task action parameters
  name: fail_task
  type: object
- description: Whether to expand inline JSON strings
  name: expandInlineJSON
  type: boolean
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-event-handler-action-schema.json
slug: conductor-conductor-event-handler-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventHandlerAction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The action type\"\n    },\n    \"start_workflow\": {\n      \"type\": \"object\",\n      \"description\": \"Start workflow action parameters\"\n    },\n    \"complete_task\": {\n      \"type\": \"object\",\n      \"description\": \"Complete task action parameters\"\n    },\n    \"fail_task\": {\n      \"type\": \"object\",\n      \"description\": \"Fail task action parameters\"\n    },\n    \"expandInlineJSON\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to expand inline JSON strings\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-event-handler-action-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: EventHandlerAction
---
