---
description: Response after adding users or teams to the Copilot subscription.
layout: schema
name: SeatsCreatedResponse
properties_list:
- description: The number of new Copilot seats created.
  name: seats_created
  type: integer
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-seats-created-response-schema.json
slug: github-copilot-seats-created-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SeatsCreatedResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response after adding users or teams to the Copilot subscription.\",\n  \"properties\": {\n    \"seats_created\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of new Copilot seats created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-seats-created-response-schema.json
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
title: SeatsCreatedResponse
---
