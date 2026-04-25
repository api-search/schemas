---
description: A Rebalancing Schedule defines a recurring job that periodically optimizes cluster node allocation for cost efficiency.
layout: schema
name: CAST AI Rebalancing Schedule
properties_list:
- description: Unique identifier for the rebalancing schedule.
  name: id
  type: string
- description: ID of the cluster this schedule applies to.
  name: clusterId
  type: string
- description: Cron expression defining when rebalancing runs.
  name: schedule
  type: string
- description: Whether the rebalancing schedule is active.
  name: enabled
  type: boolean
- description: Timestamp when the schedule was created.
  name: createdAt
  type: string
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/rebalancing-schedule.json
slug: rebalancing-schedule
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Rebalancing Schedule
---
