---
description: ''
layout: schema
name: WorkflowSummary
properties_list:
- description: ''
  name: workflowId
  type: string
- description: ''
  name: workflowType
  type: string
- description: ''
  name: version
  type: integer
- description: ''
  name: correlationId
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: updateTime
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: input
  type: string
- description: ''
  name: output
  type: string
- description: ''
  name: reasonForIncompletion
  type: string
- description: ''
  name: executionTime
  type: integer
- description: ''
  name: event
  type: string
- description: ''
  name: failedReferenceTaskNames
  type: string
- description: ''
  name: priority
  type: integer
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-workflow-summary-schema.json
slug: conductor-conductor-workflow-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"string\"\n    },\n    \"workflowType\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"integer\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\"\n    },\n    \"endTime\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"input\": {\n      \"type\": \"string\"\n    },\n    \"output\": {\n      \"type\": \"string\"\n    },\n    \"reasonForIncompletion\": {\n      \"type\": \"string\"\n    },\n    \"executionTime\": {\n      \"type\": \"integer\"\n    },\n    \"event\": {\n      \"type\": \"string\"\n    },\n    \"failedReferenceTaskNames\": {\n      \"type\": \"string\"\n    },\n \
  \   \"priority\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-workflow-summary-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: WorkflowSummary
---
