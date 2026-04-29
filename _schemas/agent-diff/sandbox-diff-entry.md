---
description: DiffEntry schema from Agent Diff API
layout: schema
name: DiffEntry
properties_list:
- description: Unique diff identifier.
  name: id
  type: string
- description: Sandbox that produced this diff.
  name: sandbox_id
  type: string
- description: API operation that triggered the state change.
  name: operation
  type: string
- description: When the operation occurred.
  name: timestamp
  type: string
- description: ''
  name: changes
  type: array
provider_name: Agent Diff
provider_slug: agent-diff
schema_file: json-schema/sandbox-diff-entry-schema.json
slug: sandbox-diff-entry
source_filename: sandbox-diff-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-diff-entry-schema.json\",\n  \"title\": \"DiffEntry\",\n  \"description\": \"DiffEntry schema from Agent Diff API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique diff identifier.\",\n      \"example\": \"500123\"\n    },\n    \"sandbox_id\": {\n      \"type\": \"string\",\n      \"description\": \"Sandbox that produced this diff.\",\n      \"example\": \"500123\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"API operation that triggered the state change.\",\n      \"example\": \"example_value\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the operation occurred.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\
  \n    },\n    \"changes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"path\": {\n            \"type\": \"string\",\n            \"description\": \"JSON path to the changed resource.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"add\",\n              \"remove\",\n              \"replace\"\n            ],\n            \"description\": \"Type of change.\"\n          },\n          \"value\": {\n            \"description\": \"New value (for add/replace operations).\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"path\": \"example_value\",\n          \"type\": \"add\",\n          \"value\": \"example_value\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-diff-entry-schema.json
tags:
- API Testing
- AI Agents
- Sandboxing
- API Diffing
- Developer Tools
title: DiffEntry
---
