---
description: A Budget Alert that monitors cloud spending against a defined budget threshold for a Cost Report.
layout: schema
name: Vantage Budget Alert
properties_list:
- description: The unique token identifier for the Budget Alert.
  name: token
  type: string
- description: The token of the associated Cost Report.
  name: cost_report_token
  type: string
- description: The budget amount.
  name: budget
  type: string
- description: The budget period (e.g., monthly).
  name: period
  type: string
- description: The date and time the Budget Alert was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/budget-alert.json
slug: budget-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/budget-alert.json\",\n  \"title\": \"Vantage Budget Alert\",\n  \"description\": \"A Budget Alert that monitors cloud spending against a defined budget threshold for a Cost Report.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Budget Alert.\"\n    },\n    \"cost_report_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the associated Cost Report.\"\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\": \"The budget amount.\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"The budget period (e.g., monthly).\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date\
  \ and time the Budget Alert was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/budget-alert.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Budget Alert
---
