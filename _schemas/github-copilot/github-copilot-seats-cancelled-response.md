---
description: Response after removing users or teams from the Copilot subscription.
layout: schema
name: SeatsCancelledResponse
properties_list:
- description: The number of Copilot seats set to pending cancellation.
  name: seats_cancelled
  type: integer
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-seats-cancelled-response-schema.json
slug: github-copilot-seats-cancelled-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SeatsCancelledResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response after removing users or teams from the Copilot subscription.\",\n  \"properties\": {\n    \"seats_cancelled\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of Copilot seats set to pending cancellation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-seats-cancelled-response-schema.json
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
title: SeatsCancelledResponse
---
