---
description: A list of team slugs to add or remove from the Copilot subscription.
layout: schema
name: SelectedTeamsRequest
properties_list:
- description: List of team slugs within the organization.
  name: selected_teams
  type: array
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-selected-teams-request-schema.json
slug: github-copilot-selected-teams-request
source_filename: github-copilot-selected-teams-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SelectedTeamsRequest\",\n  \"type\": \"object\",\n  \"description\": \"A list of team slugs to add or remove from the Copilot subscription.\",\n  \"properties\": {\n    \"selected_teams\": {\n      \"type\": \"array\",\n      \"description\": \"List of team slugs within the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-selected-teams-request-schema.json
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
title: SelectedTeamsRequest
---
