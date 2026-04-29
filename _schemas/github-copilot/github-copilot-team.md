---
description: A GitHub team.
layout: schema
name: Team
properties_list:
- description: Unique identifier of the team.
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: Name of the team.
  name: name
  type: string
- description: URL-friendly slug of the team name.
  name: slug
  type: string
- description: Description of the team.
  name: description
  type: '[''string'', ''null'']'
- description: ''
  name: privacy
  type: string
- description: ''
  name: notification_setting
  type: string
- description: The default permission level for the team.
  name: permission
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: members_url
  type: string
- description: ''
  name: repositories_url
  type: string
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-team-schema.json
slug: github-copilot-team
source_filename: github-copilot-team-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Team\",\n  \"type\": \"object\",\n  \"description\": \"A GitHub team.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the team.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the team.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly slug of the team name.\"\n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Description of the team.\"\n    },\n    \"privacy\": {\n      \"type\": \"string\"\n    },\n    \"notification_setting\": {\n      \"type\": \"string\"\n    },\n    \"permission\": {\n      \"type\": \"string\",\n      \"description\": \"The default permission level for the team.\"\n    },\n    \"url\": {\n      \"type\": \"string\"\
  \n    },\n    \"html_url\": {\n      \"type\": \"string\"\n    },\n    \"members_url\": {\n      \"type\": \"string\"\n    },\n    \"repositories_url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-team-schema.json
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
title: Team
---
