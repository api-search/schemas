---
description: Metrics for Copilot pull request summaries on github.com.
layout: schema
name: CopilotDotcomPullRequests
properties_list:
- description: Users who generated pull request summaries.
  name: total_engaged_users
  type: integer
- description: ''
  name: repositories
  type: array
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-copilot-dotcom-pull-requests-schema.json
slug: github-copilot-copilot-dotcom-pull-requests
source_filename: github-copilot-copilot-dotcom-pull-requests-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopilotDotcomPullRequests\",\n  \"type\": \"object\",\n  \"description\": \"Metrics for Copilot pull request summaries on github.com.\",\n  \"properties\": {\n    \"total_engaged_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Users who generated pull request summaries.\"\n    },\n    \"repositories\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-copilot-dotcom-pull-requests-schema.json
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
title: CopilotDotcomPullRequests
---
