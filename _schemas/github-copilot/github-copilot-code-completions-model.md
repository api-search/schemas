---
description: Code completion metrics for a specific AI model.
layout: schema
name: CodeCompletionsModel
properties_list:
- description: Name of the model or "default".
  name: name
  type: string
- description: Whether this is a custom fine-tuned model.
  name: is_custom_model
  type: boolean
- description: Training date of the custom model, if applicable.
  name: custom_model_training_date
  type: '[''string'', ''null'']'
- description: ''
  name: total_engaged_users
  type: integer
- description: ''
  name: languages
  type: array
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-code-completions-model-schema.json
slug: github-copilot-code-completions-model
source_filename: github-copilot-code-completions-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CodeCompletionsModel\",\n  \"type\": \"object\",\n  \"description\": \"Code completion metrics for a specific AI model.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the model or \\\"default\\\".\"\n    },\n    \"is_custom_model\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a custom fine-tuned model.\"\n    },\n    \"custom_model_training_date\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Training date of the custom model, if applicable.\"\n    },\n    \"total_engaged_users\": {\n      \"type\": \"integer\"\n    },\n    \"languages\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-code-completions-model-schema.json
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
title: CodeCompletionsModel
---
