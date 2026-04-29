---
description: A Conductor event handler definition that specifies how to respond to events by triggering workflows, completing tasks, or failing tasks based on configurable conditions.
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
schema_file: json-schema/event-handler.json
slug: event-handler
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/event-handler.json\",\n  \"title\": \"EventHandler\",\n  \"description\": \"A Conductor event handler definition that specifies how to respond to events by triggering workflows, completing tasks, or failing tasks based on configurable conditions.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"event\",\n    \"actions\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the event handler\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"description\": \"Event identifier in the format source:sink:subject (e.g., conductor:workflow_completed:myWorkflow)\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"description\": \"Condition expression to evaluate\"\n    },\n    \"actions\": {\n      \"type\": \"\
  array\",\n      \"description\": \"List of actions to perform when the event is received\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EventHandlerAction\"\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the event handler is active\",\n      \"default\": true\n    },\n    \"evaluatorType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of evaluator for the condition\"\n    }\n  },\n  \"$defs\": {\n    \"EventHandlerAction\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"string\",\n          \"description\": \"The action type\",\n          \"enum\": [\n            \"start_workflow\",\n            \"complete_task\",\n            \"fail_task\"\n          ]\n        },\n        \"start_workflow\": {\n          \"type\": \"object\",\n          \"description\": \"Start workflow action parameters\",\n          \"properties\": {\n            \"name\": {\n          \
  \    \"type\": \"string\",\n              \"description\": \"Name of the workflow to start\"\n            },\n            \"version\": {\n              \"type\": \"integer\",\n              \"description\": \"Version of the workflow to start\"\n            },\n            \"correlationId\": {\n              \"type\": \"string\",\n              \"description\": \"Correlation ID for the started workflow\"\n            },\n            \"input\": {\n              \"type\": \"object\",\n              \"description\": \"Input parameters for the workflow\",\n              \"additionalProperties\": true\n            }\n          }\n        },\n        \"complete_task\": {\n          \"type\": \"object\",\n          \"description\": \"Complete task action parameters\",\n          \"properties\": {\n            \"workflowId\": {\n              \"type\": \"string\",\n              \"description\": \"Workflow instance ID\"\n            },\n            \"taskRefName\": {\n              \"type\": \"\
  string\",\n              \"description\": \"Task reference name\"\n            },\n            \"output\": {\n              \"type\": \"object\",\n              \"description\": \"Output data for the completed task\",\n              \"additionalProperties\": true\n            }\n          }\n        },\n        \"fail_task\": {\n          \"type\": \"object\",\n          \"description\": \"Fail task action parameters\",\n          \"properties\": {\n            \"workflowId\": {\n              \"type\": \"string\",\n              \"description\": \"Workflow instance ID\"\n            },\n            \"taskRefName\": {\n              \"type\": \"string\",\n              \"description\": \"Task reference name\"\n            },\n            \"output\": {\n              \"type\": \"object\",\n              \"description\": \"Output data for the failed task\",\n              \"additionalProperties\": true\n            }\n          }\n        },\n        \"expandInlineJSON\": {\n          \"\
  type\": \"boolean\",\n          \"description\": \"Whether to expand inline JSON strings\",\n          \"default\": false\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/event-handler.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: EventHandler
---
