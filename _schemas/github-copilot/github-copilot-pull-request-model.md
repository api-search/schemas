---
description: Pull request summary metrics for a specific AI model.
layout: schema
name: PullRequestModel
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
- description: Total number of pull request summaries generated.
  name: total_pr_summaries_created
  type: integer
- description: ''
  name: total_engaged_users
  type: integer
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-pull-request-model-schema.json
slug: github-copilot-pull-request-model
source_filename: github-copilot-pull-request-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PullRequestModel\",\n  \"type\": \"object\",\n  \"description\": \"Pull request summary metrics for a specific AI model.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"is_custom_model\": {\n      \"type\": \"boolean\"\n    },\n    \"custom_model_training_date\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"total_pr_summaries_created\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of pull request summaries generated.\"\n    },\n    \"total_engaged_users\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-pull-request-model-schema.json
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
title: PullRequestModel
---
