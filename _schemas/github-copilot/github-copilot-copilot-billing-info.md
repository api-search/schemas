---
description: Copilot billing and subscription information for an organization, including seat breakdown and feature policy settings.
layout: schema
name: CopilotBillingInfo
properties_list:
- description: How Copilot seats are managed for the organization.
  name: seat_management_setting
  type: string
- description: Policy for Copilot Chat in IDEs.
  name: ide_chat
  type: string
- description: Policy for Copilot Chat on github.com.
  name: platform_chat
  type: string
- description: Policy for Copilot in the CLI.
  name: cli
  type: string
- description: Policy for suggestions matching public code.
  name: public_code_suggestions
  type: string
- description: The Copilot plan type for the organization.
  name: plan_type
  type: string
provider_name: GitHub Copilot
provider_slug: github-copilot
schema_file: json-schema/github-copilot-copilot-billing-info-schema.json
slug: github-copilot-copilot-billing-info
source_filename: github-copilot-copilot-billing-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CopilotBillingInfo\",\n  \"type\": \"object\",\n  \"description\": \"Copilot billing and subscription information for an organization, including seat breakdown and feature policy settings.\",\n  \"properties\": {\n    \"seat_management_setting\": {\n      \"type\": \"string\",\n      \"description\": \"How Copilot seats are managed for the organization.\"\n    },\n    \"ide_chat\": {\n      \"type\": \"string\",\n      \"description\": \"Policy for Copilot Chat in IDEs.\"\n    },\n    \"platform_chat\": {\n      \"type\": \"string\",\n      \"description\": \"Policy for Copilot Chat on github.com.\"\n    },\n    \"cli\": {\n      \"type\": \"string\",\n      \"description\": \"Policy for Copilot in the CLI.\"\n    },\n    \"public_code_suggestions\": {\n      \"type\": \"string\",\n      \"description\": \"Policy for suggestions matching public code.\"\n    },\n    \"plan_type\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The Copilot plan type for the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/json-schema/github-copilot-copilot-billing-info-schema.json
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
title: CopilotBillingInfo
---
