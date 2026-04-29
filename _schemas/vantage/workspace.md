---
description: A Workspace that serves as an organizational container for teams, reports, and other Vantage resources.
layout: schema
name: Vantage Workspace
properties_list:
- description: The unique token identifier for the Workspace.
  name: token
  type: string
- description: The name of the Workspace.
  name: name
  type: string
- description: The date and time the Workspace was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/workspace.json
slug: workspace
source_filename: workspace.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/workspace.json\",\n  \"title\": \"Vantage Workspace\",\n  \"description\": \"A Workspace that serves as an organizational container for teams, reports, and other Vantage resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Workspace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Workspace.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the Workspace was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/workspace.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Workspace
---
