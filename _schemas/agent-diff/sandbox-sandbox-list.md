---
description: SandboxList schema from Agent Diff API
layout: schema
name: SandboxList
properties_list:
- description: ''
  name: sandboxes
  type: array
- description: Total number of matching sandboxes.
  name: total
  type: integer
provider_name: Agent Diff
provider_slug: agent-diff
schema_file: json-schema/sandbox-sandbox-list-schema.json
slug: sandbox-sandbox-list
source_filename: sandbox-sandbox-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-sandbox-list-schema.json\",\n  \"title\": \"SandboxList\",\n  \"description\": \"SandboxList schema from Agent Diff API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sandboxes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Sandbox\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching sandboxes.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-sandbox-list-schema.json
tags:
- API Testing
- AI Agents
- Sandboxing
- API Diffing
- Developer Tools
title: SandboxList
---
