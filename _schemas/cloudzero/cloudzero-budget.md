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
