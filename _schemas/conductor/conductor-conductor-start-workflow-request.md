---
description: ''
layout: schema
name: StartWorkflowRequest
properties_list:
- description: Name of the workflow to start
  name: name
  type: string
- description: Version of the workflow
  name: version
  type: integer
- description: Correlation ID for the workflow instance
  name: correlationId
  type: string
- description: Priority of the workflow (0-99)
  name: priority
  type: integer
- description: Input parameters for the workflow
  name: input
  type: object
- description: Task to domain mapping for routing
  name: taskToDomain
  type: object
- description: Path to externally stored input payload
  name: externalInputPayloadStoragePath
  type: string
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/conductor-conductor-start-workflow-request-schema.json
slug: conductor-conductor-start-workflow-request
source_filename: conductor-conductor-start-workflow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StartWorkflowRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow to start\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version of the workflow\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation ID for the workflow instance\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority of the workflow (0-99)\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters for the workflow\"\n    },\n    \"taskToDomain\": {\n      \"type\": \"object\",\n      \"description\": \"Task to domain mapping for routing\"\n    },\n    \"externalInputPayloadStoragePath\": {\n      \"type\": \"string\",\n      \"description\": \"Path to externally stored\
  \ input payload\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-start-workflow-request-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: StartWorkflowRequest
---
