---
description: IDE Chat metrics for a specific editor.
layout: schema
name: IdeChatEditor
properties_list:
- description: Name of the editor.
  name: name
  type: string
- description: ''
  name: total_engaged_users
  type: integer
- description: ''
  name: models
  type: array
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-ide-chat-editor-schema.json
slug: github-copilot-ide-chat-editor
source_filename: github-copilot-ide-chat-editor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IdeChatEditor\",\n  \"type\": \"object\",\n  \"description\": \"IDE Chat metrics for a specific editor.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the editor.\"\n    },\n    \"total_engaged_users\": {\n      \"type\": \"integer\"\n    },\n    \"models\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-ide-chat-editor-schema.json
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
title: IdeChatEditor
---
