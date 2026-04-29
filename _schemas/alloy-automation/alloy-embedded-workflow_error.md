---
description: A workflow execution error record
layout: schema
name: WorkflowError
properties_list:
- description: Unique identifier for the error
  name: errorId
  type: string
- description: Workflow identifier where the error occurred
  name: workflowId
  type: string
- description: Human-readable error description
  name: message
  type: string
- description: Timestamp when the error occurred
  name: occurredAt
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-workflow_error-schema.json
slug: alloy-embedded-workflow_error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-workflow_error-schema.json\",\n  \"title\": \"WorkflowError\",\n  \"type\": \"object\",\n  \"description\": \"A workflow execution error record\",\n  \"properties\": {\n    \"errorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the error\"\n    },\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"Workflow identifier where the error occurred\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description\"\n    },\n    \"occurredAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the error occurred\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-workflow_error-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: WorkflowError
---
