---
description: Metrics for Copilot code completions in IDEs.
layout: schema
name: CopilotIdeCodeCompletions
properties_list:
- description: Users who accepted at least one code suggestion.
  name: total_engaged_users
  type: integer
- description: ''
  name: languages
  type: array
- description: ''
  name: editors
  type: array
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-copilot-ide-code-completions-schema.json
slug: github-copilot-copilot-ide-code-completions
source_filename: github-copilot-copilot-ide-code-completions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopilotIdeCodeCompletions\",\n  \"type\": \"object\",\n  \"description\": \"Metrics for Copilot code completions in IDEs.\",\n  \"properties\": {\n    \"total_engaged_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Users who accepted at least one code suggestion.\"\n    },\n    \"languages\": {\n      \"type\": \"array\"\n    },\n    \"editors\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-copilot-ide-code-completions-schema.json
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
title: CopilotIdeCodeCompletions
---
