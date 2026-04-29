---
description: A list of usernames to add or remove from the Copilot subscription.
layout: schema
name: SelectedUsersRequest
properties_list:
- description: List of GitHub usernames who are organization members.
  name: selected_usernames
  type: array
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-selected-users-request-schema.json
slug: github-copilot-selected-users-request
source_filename: github-copilot-selected-users-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SelectedUsersRequest\",\n  \"type\": \"object\",\n  \"description\": \"A list of usernames to add or remove from the Copilot subscription.\",\n  \"properties\": {\n    \"selected_usernames\": {\n      \"type\": \"array\",\n      \"description\": \"List of GitHub usernames who are organization members.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-selected-users-request-schema.json
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
title: SelectedUsersRequest
---
