---
description: A Dashboard that provides a visual overview of cloud cost data through configurable widgets.
layout: schema
name: Vantage Dashboard
properties_list:
- description: The unique token identifier for the Dashboard.
  name: token
  type: string
- description: The title of the Dashboard.
  name: title
  type: string
- description: Tokens of widgets included in the Dashboard.
  name: widget_tokens
  type: array
- description: The token of the Workspace this Dashboard belongs to.
  name: workspace_token
  type: string
- description: The date and time the Dashboard was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/dashboard.json
slug: dashboard
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/dashboard.json\",\n  \"title\": \"Vantage Dashboard\",\n  \"description\": \"A Dashboard that provides a visual overview of cloud cost data through configurable widgets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Dashboard.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Dashboard.\"\n    },\n    \"widget_tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tokens of widgets included in the Dashboard.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace this Dashboard belongs to.\"\n    },\n    \"created_at\": {\n      \"type\":\
  \ \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the Dashboard was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/dashboard.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Dashboard
---
