---
description: A Network Flow Report that tracks and analyzes network traffic costs across cloud infrastructure.
layout: schema
name: Vantage Network Flow Report
properties_list:
- description: The unique token identifier for the Network Flow Report.
  name: token
  type: string
- description: The title of the Network Flow Report.
  name: title
  type: string
- description: The token of the Workspace this report belongs to.
  name: workspace_token
  type: string
- description: The date and time the report was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/network-flow-report.json
slug: network-flow-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/network-flow-report.json\",\n  \"title\": \"Vantage Network Flow Report\",\n  \"description\": \"A Network Flow Report that tracks and analyzes network traffic costs across cloud infrastructure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Network Flow Report.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Network Flow Report.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace this report belongs to.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the report was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/network-flow-report.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Network Flow Report
---
