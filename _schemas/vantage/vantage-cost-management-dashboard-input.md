---
description: ''
layout: schema
name: DashboardInput
properties_list:
- description: The title of the Dashboard.
  name: title
  type: string
- description: Tokens of widgets to include.
  name: widget_tokens
  type: array
- description: The token of the Workspace for the Dashboard.
  name: workspace_token
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-dashboard-input-schema.json
slug: vantage-cost-management-dashboard-input
source_filename: vantage-cost-management-dashboard-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DashboardInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Dashboard.\"\n    },\n    \"widget_tokens\": {\n      \"type\": \"array\",\n      \"description\": \"Tokens of widgets to include.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace for the Dashboard.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-dashboard-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: DashboardInput
---
