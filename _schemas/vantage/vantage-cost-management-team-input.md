---
description: ''
layout: schema
name: TeamInput
properties_list:
- description: The name of the Team.
  name: name
  type: string
- description: The description of the Team.
  name: description
  type: string
- description: The token of the Workspace for the Team.
  name: workspace_token
  type: string
- description: Tokens of users to add to the Team.
  name: user_tokens
  type: array
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-team-input-schema.json
slug: vantage-cost-management-team-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TeamInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Team.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the Team.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace for the Team.\"\n    },\n    \"user_tokens\": {\n      \"type\": \"array\",\n      \"description\": \"Tokens of users to add to the Team.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-team-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: TeamInput
---
