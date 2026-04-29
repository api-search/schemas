---
description: Pull request summary metrics for a specific repository.
layout: schema
name: PullRequestRepository
properties_list:
- description: Repository name.
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
schema_file: json-schema/github-copilot-pull-request-repository-schema.json
slug: github-copilot-pull-request-repository
source_filename: github-copilot-pull-request-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PullRequestRepository\",\n  \"type\": \"object\",\n  \"description\": \"Pull request summary metrics for a specific repository.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Repository name.\"\n    },\n    \"total_engaged_users\": {\n      \"type\": \"integer\"\n    },\n    \"models\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-pull-request-repository-schema.json
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
title: PullRequestRepository
---
