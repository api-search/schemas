---
description: Represents a budget for tracking cloud spend against defined thresholds with notification rules.
layout: schema
name: CloudZero Budget
properties_list:
- description: Unique identifier for the budget.
  name: id
  type: string
- description: Display name for the budget.
  name: name
  type: string
- description: Budget amount in dollars.
  name: amount
  type: number
- description: Budget period defining the time window for tracking spend.
  name: period
  type: string
- description: Identifier for the linked View that defines the cost scope.
  name: view_id
  type: string
- description: Notification rules triggered when spend reaches defined thresholds.
  name: notifications
  type: array
- description: Timestamp when the budget was created.
  name: created_at
  type: string
- description: Timestamp when the budget was last updated.
  name: updated_at
  type: string
provider_name: CloudZero
provider_slug: cloudzero
schema_file: json-schema/cloudzero-budget.json
slug: cloudzero-budget
source_filename: cloudzero-budget.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cloudzero/blob/main/json-schema/cloudzero-budget.json\",\n  \"title\": \"CloudZero Budget\",\n  \"description\": \"Represents a budget for tracking cloud spend against defined thresholds with notification rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the budget.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the budget.\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Budget amount in dollars.\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"monthly\",\n        \"quarterly\",\n        \"annual\"\n      ],\n      \"description\": \"Budget period defining the time window for tracking spend.\"\n    },\n    \"\
  view_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the linked View that defines the cost scope.\"\n    },\n    \"notifications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"threshold\": {\n            \"type\": \"number\",\n            \"format\": \"double\",\n            \"description\": \"Threshold percentage that triggers the notification.\"\n          },\n          \"recipients\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Email addresses for notification recipients.\"\n          }\n        },\n        \"required\": [\n          \"threshold\",\n          \"recipients\"\n        ]\n      },\n      \"description\": \"Notification rules triggered when spend reaches defined thresholds.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Timestamp when the budget was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the budget was last updated.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"amount\",\n    \"period\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/json-schema/cloudzero-budget.json
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
title: CloudZero Budget
---
