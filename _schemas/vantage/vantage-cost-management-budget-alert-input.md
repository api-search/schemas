---
description: ''
layout: schema
name: BudgetAlertInput
properties_list:
- description: The token of the Cost Report to set the budget for.
  name: cost_report_token
  type: string
- description: The budget amount.
  name: budget
  type: string
- description: The budget period (e.g., monthly).
  name: period
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-budget-alert-input-schema.json
slug: vantage-cost-management-budget-alert-input
source_filename: vantage-cost-management-budget-alert-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BudgetAlertInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cost_report_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Cost Report to set the budget for.\"\n    },\n    \"budget\": {\n      \"type\": \"string\",\n      \"description\": \"The budget amount.\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"The budget period (e.g., monthly).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-budget-alert-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: BudgetAlertInput
---
