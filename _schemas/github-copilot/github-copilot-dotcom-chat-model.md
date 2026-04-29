---
description: Dotcom Chat metrics for a specific AI model.
layout: schema
name: DotcomChatModel
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: is_custom_model
  type: boolean
- description: ''
  name: custom_model_training_date
  type: '[''string'', ''null'']'
- description: ''
  name: total_engaged_users
  type: integer
- description: ''
  name: total_chats
  type: integer
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-dotcom-chat-model-schema.json
slug: github-copilot-dotcom-chat-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DotcomChatModel\",\n  \"type\": \"object\",\n  \"description\": \"Dotcom Chat metrics for a specific AI model.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"is_custom_model\": {\n      \"type\": \"boolean\"\n    },\n    \"custom_model_training_date\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"total_engaged_users\": {\n      \"type\": \"integer\"\n    },\n    \"total_chats\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-dotcom-chat-model-schema.json
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
title: DotcomChatModel
---
