---
description: Represents the status and result of a Restack long-running workflow execution.
layout: schema
name: Workflow Run
properties_list:
- description: Unique identifier for the workflow run.
  name: runId
  type: string
- description: The name of the workflow that was executed.
  name: workflowName
  type: string
- description: Current execution status of the workflow run.
  name: status
  type: string
- description: Input parameters provided when scheduling the workflow.
  name: input
  type: object
- description: Output returned by the workflow upon completion.
  name: output
  type: object
- description: Error message if the workflow run failed.
  name: error
  type: string
- description: ISO 8601 timestamp when the workflow run was created.
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the workflow run completed.
  name: completedAt
  type: string
provider_name: Restack
provider_slug: restack
schema_file: json-schema/restack-workflow-run-schema.json
slug: restack-workflow-run
source_filename: restack-workflow-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/restack/refs/heads/main/json-schema/restack-workflow-run-schema.json\",\n  \"title\": \"Workflow Run\",\n  \"description\": \"Represents the status and result of a Restack long-running workflow execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the workflow run.\",\n      \"pattern\": \"^run_[a-zA-Z0-9_]+$\"\n    },\n    \"workflowName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow that was executed.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current execution status of the workflow run.\",\n      \"enum\": [\"queued\", \"running\", \"completed\", \"failed\"]\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters provided when\
  \ scheduling the workflow.\",\n      \"additionalProperties\": true\n    },\n    \"output\": {\n      \"type\": \"object\",\n      \"description\": \"Output returned by the workflow upon completion.\",\n      \"additionalProperties\": true\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the workflow run failed.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the workflow run was created.\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the workflow run completed.\"\n    }\n  },\n  \"required\": [\"runId\", \"workflowName\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restack/refs/heads/main/json-schema/restack-workflow-run-schema.json
tags:
- AI Agents
- Workflows
- Orchestration
- Enterprise
- Python
title: Workflow Run
---
