---
description: Detailed code completion metrics for a specific language.
layout: schema
name: CodeCompletionsLanguageMetrics
properties_list:
- description: Programming language name.
  name: name
  type: string
- description: ''
  name: total_engaged_users
  type: integer
- description: Total number of code suggestions shown.
  name: total_code_suggestions
  type: integer
- description: Total number of code suggestions accepted.
  name: total_code_acceptances
  type: integer
- description: Total lines of code suggested.
  name: total_code_lines_suggested
  type: integer
- description: Total lines of code accepted.
  name: total_code_lines_accepted
  type: integer
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-code-completions-language-metrics-schema.json
slug: github-copilot-code-completions-language-metrics
source_filename: github-copilot-code-completions-language-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CodeCompletionsLanguageMetrics\",\n  \"type\": \"object\",\n  \"description\": \"Detailed code completion metrics for a specific language.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Programming language name.\"\n    },\n    \"total_engaged_users\": {\n      \"type\": \"integer\"\n    },\n    \"total_code_suggestions\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of code suggestions shown.\"\n    },\n    \"total_code_acceptances\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of code suggestions accepted.\"\n    },\n    \"total_code_lines_suggested\": {\n      \"type\": \"integer\",\n      \"description\": \"Total lines of code suggested.\"\n    },\n    \"total_code_lines_accepted\": {\n      \"type\": \"integer\",\n      \"description\": \"Total lines of code accepted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-code-completions-language-metrics-schema.json
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
title: CodeCompletionsLanguageMetrics
---
