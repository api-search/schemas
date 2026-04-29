---
description: A Cost Report in Vantage that tracks and visualizes cloud spending using VQL filters and groupings across providers.
layout: schema
name: Vantage Cost Report
properties_list:
- description: The unique token identifier for the Cost Report.
  name: token
  type: string
- description: The title of the Cost Report.
  name: title
  type: string
- description: The VQL filter applied to the Cost Report.
  name: filter
  type: string
- description: The groupings applied to the Cost Report.
  name: groupings
  type: string
- description: The token of the Folder this report belongs to.
  name: folder_token
  type: string
- description: Tokens of Saved Filters applied to this report.
  name: saved_filter_tokens
  type: array
- description: The token of the Workspace this report belongs to.
  name: workspace_token
  type: string
- description: The date and time the Cost Report was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/cost-report.json
slug: cost-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/cost-report.json\",\n  \"title\": \"Vantage Cost Report\",\n  \"description\": \"A Cost Report in Vantage that tracks and visualizes cloud spending using VQL filters and groupings across providers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Cost Report.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Cost Report.\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"The VQL filter applied to the Cost Report.\"\n    },\n    \"groupings\": {\n      \"type\": \"string\",\n      \"description\": \"The groupings applied to the Cost Report.\"\n    },\n    \"folder_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the\
  \ Folder this report belongs to.\"\n    },\n    \"saved_filter_tokens\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tokens of Saved Filters applied to this report.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace this report belongs to.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the Cost Report was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/cost-report.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Cost Report
---
