---
description: A workflow execution log entry
layout: schema
name: WorkflowLog
properties_list:
- description: Unique identifier for the log entry
  name: logId
  type: string
- description: Workflow identifier
  name: workflowId
  type: string
- description: Execution status
  name: status
  type: string
- description: Timestamp when the workflow was executed
  name: executedAt
  type: string
- description: Execution duration in milliseconds
  name: duration
  type: integer
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-embedded-workflow_log-schema.json
slug: alloy-embedded-workflow_log
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-embedded-workflow_log-schema.json\",\n  \"title\": \"WorkflowLog\",\n  \"type\": \"object\",\n  \"description\": \"A workflow execution log entry\",\n  \"properties\": {\n    \"logId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the log entry\"\n    },\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"Workflow identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Execution status\",\n      \"enum\": [\n        \"success\",\n        \"failure\",\n        \"pending\"\n      ]\n    },\n    \"executedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the workflow was executed\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Execution duration in milliseconds\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-embedded-workflow_log-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: WorkflowLog
---
