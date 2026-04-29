---
description: Sandbox schema from Agent Diff API
layout: schema
name: Sandbox
properties_list:
- description: Unique sandbox identifier.
  name: id
  type: string
- description: The third-party API being sandboxed.
  name: api
  type: string
- description: Scenario name for this sandbox.
  name: scenario
  type: string
- description: Current sandbox status.
  name: status
  type: string
- description: Base URL for interacting with the sandbox replica.
  name: base_url
  type: string
- description: When the sandbox was created.
  name: created_at
  type: string
- description: When the sandbox will expire.
  name: expires_at
  type: string
provider_name: Agent Diff
provider_slug: agent-diff
schema_file: json-schema/sandbox-sandbox-schema.json
slug: sandbox-sandbox
source_filename: sandbox-sandbox-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-sandbox-schema.json\",\n  \"title\": \"Sandbox\",\n  \"description\": \"Sandbox schema from Agent Diff API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique sandbox identifier.\",\n      \"example\": \"500123\"\n    },\n    \"api\": {\n      \"type\": \"string\",\n      \"description\": \"The third-party API being sandboxed.\",\n      \"example\": \"example_value\"\n    },\n    \"scenario\": {\n      \"type\": \"string\",\n      \"description\": \"Scenario name for this sandbox.\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ready\",\n        \"active\",\n        \"expired\",\n        \"deleted\"\n      ],\n      \"description\": \"Current sandbox\
  \ status.\",\n      \"example\": \"ready\"\n    },\n    \"base_url\": {\n      \"type\": \"string\",\n      \"description\": \"Base URL for interacting with the sandbox replica.\",\n      \"example\": \"https://example.com\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the sandbox was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the sandbox will expire.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-sandbox-schema.json
tags:
- API Testing
- AI Agents
- Sandboxing
- API Diffing
- Developer Tools
title: Sandbox
---
