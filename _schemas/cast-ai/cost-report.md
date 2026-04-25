---
description: A Cost Report provides efficiency metrics and cost data for a cluster, including CPU and memory utilization and potential savings.
layout: schema
name: CAST AI Cost Report
properties_list:
- description: ID of the cluster this report covers.
  name: clusterId
  type: string
- description: CPU efficiency percentage (0-100).
  name: cpuEfficiency
  type: number
- description: Memory efficiency percentage (0-100).
  name: memoryEfficiency
  type: number
- description: Total monthly cost in USD before optimization.
  name: totalMonthlyCost
  type: number
- description: Projected monthly cost in USD after optimization.
  name: optimizedMonthlyCost
  type: number
- description: Percentage of costs saved through optimization.
  name: savingsPercentage
  type: number
provider_name: CAST AI
provider_slug: cast-ai
schema_file: json-schema/cost-report.json
slug: cost-report
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
title: CAST AI Cost Report
---
