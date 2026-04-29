---
description: ''
layout: schema
name: SavedFilter
properties_list:
- description: The unique token identifier for the Saved Filter.
  name: token
  type: string
- description: The title of the Saved Filter.
  name: title
  type: string
- description: The VQL filter expression.
  name: filter
  type: string
- description: The token of the Workspace this Saved Filter belongs to.
  name: workspace_token
  type: string
- description: The date and time the Saved Filter was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-saved-filter-schema.json
slug: vantage-cost-management-saved-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SavedFilter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Saved Filter.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Saved Filter.\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"The VQL filter expression.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace this Saved Filter belongs to.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the Saved Filter was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-saved-filter-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: SavedFilter
---
