---
description: Represents a cost insight for tracking cost anomalies and patterns within CloudZero.
layout: schema
name: CloudZero Insight
properties_list:
- description: Unique identifier for the insight.
  name: id
  type: string
- description: Display name for the insight.
  name: name
  type: string
- description: Description of what the insight tracks.
  name: description
  type: string
- description: Timestamp when the insight was created.
  name: created_at
  type: string
- description: Timestamp when the insight was last updated.
  name: updated_at
  type: string
- description: Filters applied to the insight for narrowing cost data.
  name: filters
  type: object
- description: Dimensions used for grouping cost data within the insight.
  name: group_by
  type: array
provider_name: CloudZero
provider_slug: cloudzero
schema_file: json-schema/cloudzero-insight.json
slug: cloudzero-insight
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
title: CloudZero Insight
---
