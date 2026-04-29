---
description: SandboxCreateRequest schema from Agent Diff API
layout: schema
name: SandboxCreateRequest
properties_list:
- description: The third-party API to sandbox (e.g., slack, linear, github).
  name: api
  type: string
- description: Named scenario for the sandbox seed data.
  name: scenario
  type: string
- description: Initial state data to populate the sandbox.
  name: seed_data
  type: object
- description: Time-to-live in seconds before the sandbox expires.
  name: ttl
  type: integer
provider_name: Agent Diff
provider_slug: agent-diff
schema_file: json-schema/sandbox-sandbox-create-request-schema.json
slug: sandbox-sandbox-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-sandbox-create-request-schema.json\",\n  \"title\": \"SandboxCreateRequest\",\n  \"description\": \"SandboxCreateRequest schema from Agent Diff API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api\": {\n      \"type\": \"string\",\n      \"description\": \"The third-party API to sandbox (e.g., slack, linear, github).\",\n      \"example\": \"example_value\"\n    },\n    \"scenario\": {\n      \"type\": \"string\",\n      \"description\": \"Named scenario for the sandbox seed data.\",\n      \"example\": \"example_value\"\n    },\n    \"seed_data\": {\n      \"type\": \"object\",\n      \"description\": \"Initial state data to populate the sandbox.\",\n      \"example\": {}\n    },\n    \"ttl\": {\n      \"type\": \"integer\",\n      \"description\": \"Time-to-live in seconds before the sandbox\
  \ expires.\",\n      \"default\": 3600,\n      \"example\": 1\n    }\n  },\n  \"required\": [\n    \"api\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-sandbox-create-request-schema.json
tags:
- API Testing
- AI Agents
- Sandboxing
- API Diffing
- Developer Tools
title: SandboxCreateRequest
---
