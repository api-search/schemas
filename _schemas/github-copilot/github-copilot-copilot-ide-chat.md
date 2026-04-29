---
description: Metrics for Copilot Chat in IDEs.
layout: schema
name: CopilotIdeChat
properties_list:
- description: Users who prompted Copilot Chat in an IDE.
  name: total_engaged_users
  type: integer
- description: ''
  name: editors
  type: array
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-copilot-ide-chat-schema.json
slug: github-copilot-copilot-ide-chat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopilotIdeChat\",\n  \"type\": \"object\",\n  \"description\": \"Metrics for Copilot Chat in IDEs.\",\n  \"properties\": {\n    \"total_engaged_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Users who prompted Copilot Chat in an IDE.\"\n    },\n    \"editors\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-copilot-ide-chat-schema.json
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
title: CopilotIdeChat
---
