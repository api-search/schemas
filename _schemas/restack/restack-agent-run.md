---
description: Represents the status and result of a Restack AI agent execution run.
layout: schema
name: Agent Run
properties_list:
- description: Unique identifier for the agent run.
  name: runId
  type: string
- description: The name of the agent that was executed.
  name: agentName
  type: string
- description: Current execution status of the agent run.
  name: status
  type: string
- description: Input parameters provided when scheduling the agent.
  name: input
  type: object
- description: Output returned by the agent upon completion.
  name: output
  type: object
- description: Error message if the agent run failed.
  name: error
  type: string
- description: ISO 8601 timestamp when the agent run was created.
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the agent run completed.
  name: completedAt
  type: string
provider_name: Restack
provider_slug: restack
schema_file: json-schema/restack-agent-run-schema.json
slug: restack-agent-run
source_filename: restack-agent-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/restack/refs/heads/main/json-schema/restack-agent-run-schema.json\",\n  \"title\": \"Agent Run\",\n  \"description\": \"Represents the status and result of a Restack AI agent execution run.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"runId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the agent run.\",\n      \"pattern\": \"^run_[a-zA-Z0-9]+$\"\n    },\n    \"agentName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the agent that was executed.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current execution status of the agent run.\",\n      \"enum\": [\"queued\", \"running\", \"completed\", \"failed\"]\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters provided when scheduling the agent.\"\
  ,\n      \"additionalProperties\": true\n    },\n    \"output\": {\n      \"type\": \"object\",\n      \"description\": \"Output returned by the agent upon completion.\",\n      \"additionalProperties\": true\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the agent run failed.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the agent run was created.\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the agent run completed.\"\n    }\n  },\n  \"required\": [\"runId\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restack/refs/heads/main/json-schema/restack-agent-run-schema.json
tags:
- AI Agents
- Workflows
- Orchestration
- Enterprise
- Python
title: Agent Run
---
