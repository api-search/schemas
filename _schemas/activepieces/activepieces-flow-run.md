---
description: A flow execution run
layout: schema
name: FlowRun
properties_list:
- description: Flow run ID
  name: id
  type: string
- description: Run creation timestamp
  name: created
  type: string
- description: Last update timestamp
  name: updated
  type: string
- description: Project ID
  name: projectId
  type: string
- description: Flow ID
  name: flowId
  type: string
- description: Run status
  name: status
  type: string
- description: Run start time
  name: startTime
  type: string
- description: Run finish time
  name: finishTime
  type: string
- description: Execution duration in milliseconds
  name: duration
  type: integer
provider_name: Activepieces
provider_slug: activepieces
schema_file: json-schema/activepieces-flow-run-schema.json
slug: activepieces-flow-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-flow-run-schema.json\",\n  \"title\": \"FlowRun\",\n  \"description\": \"A flow execution run\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Flow run ID\",\n      \"example\": \"run-abc123\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Run creation timestamp\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Project ID\"\n    },\n    \"flowId\": {\n      \"type\": \"string\",\n      \"description\": \"Flow ID\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\n        \"RUNNING\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"TIMEOUT\",\n        \"STOPPED\"\n      ],\n      \"description\": \"Run status\",\n      \"example\": \"SUCCEEDED\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Run start time\"\n    },\n    \"finishTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Run finish time\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Execution duration in milliseconds\",\n      \"example\": 1234\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/json-schema/activepieces-flow-run-schema.json
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
title: FlowRun
---
