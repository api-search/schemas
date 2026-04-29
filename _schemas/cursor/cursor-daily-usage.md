---
description: Daily usage metrics record produced by the Cursor Admin API daily-usage-data endpoint.
layout: schema
name: Cursor Daily Usage Record
properties_list:
- description: Calendar date for the usage record.
  name: date
  type: string
- description: Identifier of the user the metrics belong to.
  name: userId
  type: string
- description: ''
  name: linesAdded
  type: integer
- description: ''
  name: linesDeleted
  type: integer
- description: ''
  name: completions
  type: integer
- description: ''
  name: chatRequests
  type: integer
- description: Map of model name to request count.
  name: modelUsage
  type: object
provider_name: Cursor
provider_slug: cursor
schema_file: json-schema/cursor-daily-usage-schema.json
slug: cursor-daily-usage
source_filename: cursor-daily-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/json-schema/cursor-daily-usage-schema.json\",\n  \"title\": \"Cursor Daily Usage Record\",\n  \"description\": \"Daily usage metrics record produced by the Cursor Admin API daily-usage-data endpoint.\",\n  \"type\": \"object\",\n  \"required\": [\"date\", \"userId\"],\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Calendar date for the usage record.\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user the metrics belong to.\"\n    },\n    \"linesAdded\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"linesDeleted\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"completions\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"chatRequests\"\
  : {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"modelUsage\": {\n      \"type\": \"object\",\n      \"description\": \"Map of model name to request count.\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"minimum\": 0\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cursor/refs/heads/main/json-schema/cursor-daily-usage-schema.json
tags:
- AI
- AI Editor
- Code Generation
- Coding Assistant
- Copilot
- Developer Tools
- LLM
- Productivity
- VSCode Fork
title: Cursor Daily Usage Record
---
