---
description: A recurring budget rule for controlling Kubernetes spending, with configurable thresholds and notification actions.
layout: schema
name: Kubecost Budget
properties_list:
- description: Unique identifier for the budget.
  name: id
  type: string
- description: Name of the budget rule.
  name: name
  type: string
- description: Budget amount limit.
  name: amount
  type: number
- description: Recurrence interval of the budget.
  name: interval
  type: string
- description: The field used to scope the budget, such as namespace, cluster, or label.
  name: aggregation
  type: string
- description: Filter expression to scope the budget to specific workloads.
  name: filter
  type: string
- description: Alert actions triggered when budget thresholds are reached.
  name: actions
  type: array
- description: Current spend within the budget period.
  name: currentSpend
  type: number
- description: Timestamp when the budget was created.
  name: createdAt
  type: string
- description: Timestamp when the budget was last updated.
  name: updatedAt
  type: string
provider_name: Kubecost
provider_slug: kubecost
schema_file: json-schema/budget.json
slug: budget
source_filename: budget.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kubecost/blob/main/json-schema/budget.json\",\n  \"title\": \"Kubecost Budget\",\n  \"description\": \"A recurring budget rule for controlling Kubernetes spending, with configurable thresholds and notification actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the budget.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the budget rule.\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Budget amount limit.\"\n    },\n    \"interval\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"weekly\",\n        \"monthly\"\n      ],\n      \"description\": \"Recurrence interval of the budget.\"\n    },\n    \"aggregation\": {\n      \"type\": \"string\",\n      \"description\": \"The field\
  \ used to scope the budget, such as namespace, cluster, or label.\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"Filter expression to scope the budget to specific workloads.\"\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"description\": \"Alert actions triggered when budget thresholds are reached.\",\n      \"items\": {\n        \"$ref\": \"budget-action.json\"\n      }\n    },\n    \"currentSpend\": {\n      \"type\": \"number\",\n      \"description\": \"Current spend within the budget period.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the budget was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the budget was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/json-schema/budget.json
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
title: Kubecost Budget
---
