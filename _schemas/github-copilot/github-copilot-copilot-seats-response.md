---
description: Paginated list of Copilot seat assignments.
layout: schema
name: CopilotSeatsResponse
properties_list:
- description: Total number of Copilot seats for the organization.
  name: total_seats
  type: integer
- description: ''
  name: seats
  type: array
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-copilot-seats-response-schema.json
slug: github-copilot-copilot-seats-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopilotSeatsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of Copilot seat assignments.\",\n  \"properties\": {\n    \"total_seats\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of Copilot seats for the organization.\"\n    },\n    \"seats\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-copilot-seats-response-schema.json
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
title: CopilotSeatsResponse
---
