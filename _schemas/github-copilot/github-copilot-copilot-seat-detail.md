---
description: Details of a Copilot seat assignment for a user, including activity information and plan type.
layout: schema
name: CopilotSeatDetail
properties_list:
- description: Timestamp when the seat was created.
  name: created_at
  type: string
- description: Timestamp when the seat was last updated.
  name: updated_at
  type: string
- description: Date when seat cancellation takes effect. Null if not pending cancellation.
  name: pending_cancellation_date
  type: '[''string'', ''null'']'
- description: Timestamp of the user's last Copilot activity. Null if no activity recorded.
  name: last_activity_at
  type: '[''string'', ''null'']'
- description: The IDE or editor used during the user's last Copilot activity. Null if no activity recorded.
  name: last_activity_editor
  type: '[''string'', ''null'']'
- description: Timestamp of the user's last authentication with Copilot. Null if never authenticated.
  name: last_authenticated_at
  type: '[''string'', ''null'']'
- description: The Copilot plan type for this seat.
  name: plan_type
  type: string
- description: The GitHub user assigned to this seat.
  name: assignee
  type: string
- description: The team through which this seat was assigned, if applicable.
  name: assigning_team
  type: string
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-copilot-seat-detail-schema.json
slug: github-copilot-copilot-seat-detail
source_filename: github-copilot-copilot-seat-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopilotSeatDetail\",\n  \"type\": \"object\",\n  \"description\": \"Details of a Copilot seat assignment for a user, including activity information and plan type.\",\n  \"properties\": {\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the seat was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the seat was last updated.\"\n    },\n    \"pending_cancellation_date\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date when seat cancellation takes effect. Null if not pending cancellation.\"\n    },\n    \"last_activity_at\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Timestamp of the user's last Copilot activity. Null if no activity recorded.\"\n    },\n    \"last_activity_editor\": {\n      \"type\": \"['string', 'null']\",\n      \"description\"\
  : \"The IDE or editor used during the user's last Copilot activity. Null if no activity recorded.\"\n    },\n    \"last_authenticated_at\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Timestamp of the user's last authentication with Copilot. Null if never authenticated.\"\n    },\n    \"plan_type\": {\n      \"type\": \"string\",\n      \"description\": \"The Copilot plan type for this seat.\"\n    },\n    \"assignee\": {\n      \"type\": \"string\",\n      \"description\": \"The GitHub user assigned to this seat.\"\n    },\n    \"assigning_team\": {\n      \"type\": \"string\",\n      \"description\": \"The team through which this seat was assigned, if applicable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-copilot-seat-detail-schema.json
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
title: CopilotSeatDetail
---
