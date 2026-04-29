---
description: Aggregated Copilot usage metrics for a single day, broken down by feature, editor, language, and model.
layout: schema
name: CopilotMetricsDay
properties_list:
- description: The date these metrics apply to (YYYY-MM-DD).
  name: date
  type: string
- description: Total users with any Copilot activity on this date.
  name: total_active_users
  type: integer
- description: Total users who actively engaged with Copilot features on this date.
  name: total_engaged_users
  type: integer
- description: ''
  name: copilot_ide_code_completions
  type: string
- description: ''
  name: copilot_ide_chat
  type: string
- description: ''
  name: copilot_dotcom_chat
  type: string
- description: ''
  name: copilot_dotcom_pull_requests
  type: string
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-copilot-metrics-day-schema.json
slug: github-copilot-copilot-metrics-day
source_filename: github-copilot-copilot-metrics-day-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopilotMetricsDay\",\n  \"type\": \"object\",\n  \"description\": \"Aggregated Copilot usage metrics for a single day, broken down by feature, editor, language, and model.\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The date these metrics apply to (YYYY-MM-DD).\"\n    },\n    \"total_active_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Total users with any Copilot activity on this date.\"\n    },\n    \"total_engaged_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Total users who actively engaged with Copilot features on this date.\"\n    },\n    \"copilot_ide_code_completions\": {\n      \"type\": \"string\"\n    },\n    \"copilot_ide_chat\": {\n      \"type\": \"string\"\n    },\n    \"copilot_dotcom_chat\": {\n      \"type\": \"string\"\n    },\n    \"copilot_dotcom_pull_requests\": {\n      \"type\"\
  : \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-copilot-metrics-day-schema.json
tags:
- Agents
- AI
- Artificial Intelligence
- Code Generation
- Code Review
- Coding Agent
- Custom Instructions
- Developer Tools
- Extensions
- IDE
- Machine Learning
- MCP
- Metrics
- Model Context Protocol
- Productivity
title: CopilotMetricsDay
---
