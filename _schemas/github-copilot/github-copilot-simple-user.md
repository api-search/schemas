---
description: A GitHub user account.
layout: schema
name: SimpleUser
properties_list:
- description: The username of the user.
  name: login
  type: string
- description: The unique identifier of the user.
  name: id
  type: integer
- description: The GraphQL node ID of the user.
  name: node_id
  type: string
- description: URL to the user's avatar image.
  name: avatar_url
  type: string
- description: ''
  name: gravatar_id
  type: '[''string'', ''null'']'
- description: API URL for this user.
  name: url
  type: string
- description: URL to the user's GitHub profile.
  name: html_url
  type: string
- description: ''
  name: followers_url
  type: string
- description: ''
  name: following_url
  type: string
- description: ''
  name: gists_url
  type: string
- description: ''
  name: starred_url
  type: string
- description: ''
  name: subscriptions_url
  type: string
- description: ''
  name: organizations_url
  type: string
- description: ''
  name: repos_url
  type: string
- description: ''
  name: events_url
  type: string
- description: ''
  name: received_events_url
  type: string
- description: The type of account (User, Organization, Bot, etc.).
  name: type
  type: string
- description: Whether the user is a GitHub site administrator.
  name: site_admin
  type: boolean
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-simple-user-schema.json
slug: github-copilot-simple-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SimpleUser\",\n  \"type\": \"object\",\n  \"description\": \"A GitHub user account.\",\n  \"properties\": {\n    \"login\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the user.\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the user.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL node ID of the user.\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the user's avatar image.\"\n    },\n    \"gravatar_id\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"API URL for this user.\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the user's GitHub profile.\"\n    },\n    \"followers_url\": {\n      \"type\"\
  : \"string\"\n    },\n    \"following_url\": {\n      \"type\": \"string\"\n    },\n    \"gists_url\": {\n      \"type\": \"string\"\n    },\n    \"starred_url\": {\n      \"type\": \"string\"\n    },\n    \"subscriptions_url\": {\n      \"type\": \"string\"\n    },\n    \"organizations_url\": {\n      \"type\": \"string\"\n    },\n    \"repos_url\": {\n      \"type\": \"string\"\n    },\n    \"events_url\": {\n      \"type\": \"string\"\n    },\n    \"received_events_url\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of account (User, Organization, Bot, etc.).\"\n    },\n    \"site_admin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is a GitHub site administrator.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-simple-user-schema.json
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
title: SimpleUser
---
