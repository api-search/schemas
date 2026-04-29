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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cast-ai/blob/main/json-schema/rebalancing-schedule.json\",\n  \"title\": \"CAST AI Rebalancing Schedule\",\n  \"description\": \"A Rebalancing Schedule defines a recurring job that periodically optimizes cluster node allocation for cost efficiency.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the rebalancing schedule.\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the cluster this schedule applies to.\"\n    },\n    \"schedule\": {\n      \"type\": \"string\",\n      \"description\": \"Cron expression defining when rebalancing runs.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rebalancing schedule is active.\"\n\
  \    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the schedule was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/json-schema/rebalancing-schedule.json
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
