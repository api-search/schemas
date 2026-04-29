---
description: An AWS Budget that tracks cost, usage, RI utilization, or Savings Plans coverage
layout: schema
name: AWS Budget
properties_list:
- description: The name of the budget. Must be unique within an account.
  name: BudgetName
  type: string
- description: The total amount of cost, usage, RI utilization, or Savings Plans coverage that you want to track
  name: BudgetLimit
  type: object
- description: Filters to apply to the budget (e.g., by service, region, tag)
  name: CostFilters
  type: object
- description: Cost types to include in the budget calculation
  name: CostTypes
  type: object
- description: The period covered by a budget
  name: TimeUnit
  type: string
- description: ''
  name: TimePeriod
  type: object
- description: The type of budget
  name: BudgetType
  type: string
- description: ''
  name: CalculatedSpend
  type: object
provider_name: Amazon Billing And Cost Management
provider_slug: amazon-billing-and-cost-management
schema_file: json-schema/cost-budget-schema.json
slug: cost-budget
source_filename: cost-budget-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/main/json-schema/cost-budget-schema.json\",\n  \"title\": \"AWS Budget\",\n  \"description\": \"An AWS Budget that tracks cost, usage, RI utilization, or Savings Plans coverage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BudgetName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the budget. Must be unique within an account.\",\n      \"maxLength\": 100\n    },\n    \"BudgetLimit\": {\n      \"type\": \"object\",\n      \"description\": \"The total amount of cost, usage, RI utilization, or Savings Plans coverage that you want to track\",\n      \"properties\": {\n        \"Amount\": { \"type\": \"string\", \"description\": \"The cost or usage amount\" },\n        \"Unit\": { \"type\": \"string\", \"description\": \"Currency unit (e.g., USD)\" }\n      },\n      \"required\": [\"\
  Amount\", \"Unit\"]\n    },\n    \"CostFilters\": {\n      \"type\": \"object\",\n      \"description\": \"Filters to apply to the budget (e.g., by service, region, tag)\"\n    },\n    \"CostTypes\": {\n      \"type\": \"object\",\n      \"description\": \"Cost types to include in the budget calculation\",\n      \"properties\": {\n        \"IncludeTax\": { \"type\": \"boolean\" },\n        \"IncludeSubscription\": { \"type\": \"boolean\" },\n        \"UseBlended\": { \"type\": \"boolean\" },\n        \"IncludeRefund\": { \"type\": \"boolean\" },\n        \"IncludeCredit\": { \"type\": \"boolean\" },\n        \"IncludeUpfront\": { \"type\": \"boolean\" },\n        \"IncludeRecurring\": { \"type\": \"boolean\" },\n        \"IncludeOtherSubscription\": { \"type\": \"boolean\" },\n        \"IncludeSupport\": { \"type\": \"boolean\" },\n        \"IncludeDiscount\": { \"type\": \"boolean\" },\n        \"UseAmortized\": { \"type\": \"boolean\" }\n      }\n    },\n    \"TimeUnit\": {\n      \"\
  type\": \"string\",\n      \"enum\": [\"DAILY\", \"MONTHLY\", \"QUARTERLY\", \"ANNUALLY\"],\n      \"description\": \"The period covered by a budget\"\n    },\n    \"TimePeriod\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Start\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"End\": { \"type\": \"string\", \"format\": \"date-time\" }\n      }\n    },\n    \"BudgetType\": {\n      \"type\": \"string\",\n      \"enum\": [\"USAGE\", \"COST\", \"RI_UTILIZATION\", \"RI_COVERAGE\", \"SAVINGS_PLANS_UTILIZATION\", \"SAVINGS_PLANS_COVERAGE\"],\n      \"description\": \"The type of budget\"\n    },\n    \"CalculatedSpend\": {\n      \"type\": \"object\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"ActualSpend\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Amount\": { \"type\": \"string\" },\n            \"Unit\": { \"type\": \"string\" }\n          }\n        },\n        \"ForecastedSpend\": {\n    \
  \      \"type\": \"object\",\n          \"properties\": {\n            \"Amount\": { \"type\": \"string\" },\n            \"Unit\": { \"type\": \"string\" }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"BudgetName\", \"TimeUnit\", \"BudgetType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/json-schema/cost-budget-schema.json
tags:
- Billing
- Cost Management
- Cost Explorer
- Budgets
- Cost Optimization
- FinOps
- Amazon Web Services
- AWS
title: AWS Budget
---
