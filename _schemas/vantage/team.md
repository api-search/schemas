---
description: A Team that groups users together for managing access to Vantage resources within a Workspace.
layout: schema
name: Vantage Team
properties_list:
- description: The unique token identifier for the Team.
  name: token
  type: string
- description: The name of the Team.
  name: name
  type: string
- description: The description of the Team.
  name: description
  type: string
- description: The token of the Workspace this Team belongs to.
  name: workspace_token
  type: string
- description: Tokens of users who are members of the Team.
  name: user_tokens
  type: array
- description: The date and time the Team was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/team.json
slug: team
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/team.json\",\n  \"title\": \"Vantage Team\",\n  \"description\": \"A Team that groups users together for managing access to Vantage resources within a Workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Team.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Team.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the Team.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace this Team belongs to.\"\n    },\n    \"user_tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tokens\
  \ of users who are members of the Team.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the Team was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/team.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Team
---
