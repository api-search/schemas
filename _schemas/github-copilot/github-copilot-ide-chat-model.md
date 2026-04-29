---
description: IDE Chat metrics for a specific AI model.
layout: schema
name: IdeChatModel
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
- description: Total number of chat conversations.
  name: total_chats
  type: integer
- description: Number of times chat suggestions were inserted into code.
  name: total_chat_insertion_events
  type: integer
- description: Number of times chat responses were copied.
  name: total_chat_copy_events
  type: integer
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-ide-chat-model-schema.json
slug: github-copilot-ide-chat-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IdeChatModel\",\n  \"type\": \"object\",\n  \"description\": \"IDE Chat metrics for a specific AI model.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"is_custom_model\": {\n      \"type\": \"boolean\"\n    },\n    \"custom_model_training_date\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"total_engaged_users\": {\n      \"type\": \"integer\"\n    },\n    \"total_chats\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of chat conversations.\"\n    },\n    \"total_chat_insertion_events\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times chat suggestions were inserted into code.\"\n    },\n    \"total_chat_copy_events\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times chat responses were copied.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-ide-chat-model-schema.json
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
title: IdeChatModel
---
