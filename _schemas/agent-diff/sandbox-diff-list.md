---
description: DiffList schema from Agent Diff API
layout: schema
name: DiffList
properties_list:
- description: ''
  name: diffs
  type: array
- description: Total number of diffs.
  name: total
  type: integer
provider_name: Agent Diff
provider_slug: agent-diff
schema_file: json-schema/sandbox-diff-list-schema.json
slug: sandbox-diff-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-diff-list-schema.json\",\n  \"title\": \"DiffList\",\n  \"description\": \"DiffList schema from Agent Diff API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"diffs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DiffEntry\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of diffs.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agent-diff/refs/heads/main/json-schema/sandbox-diff-list-schema.json
tags:
- API Testing
- AI Agents
- Sandboxing
- API Diffing
- Developer Tools
title: DiffList
---
