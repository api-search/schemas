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
source_filename: cost-report.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cast-ai/blob/main/json-schema/cost-report.json\",\n  \"title\": \"CAST AI Cost Report\",\n  \"description\": \"A Cost Report provides efficiency metrics and cost data for a cluster, including CPU and memory utilization and potential savings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the cluster this report covers.\"\n    },\n    \"cpuEfficiency\": {\n      \"type\": \"number\",\n      \"description\": \"CPU efficiency percentage (0-100).\"\n    },\n    \"memoryEfficiency\": {\n      \"type\": \"number\",\n      \"description\": \"Memory efficiency percentage (0-100).\"\n    },\n    \"totalMonthlyCost\": {\n      \"type\": \"number\",\n      \"description\": \"Total monthly cost in USD before optimization.\"\n    },\n    \"optimizedMonthlyCost\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Projected monthly cost in USD after optimization.\"\n    },\n    \"savingsPercentage\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage of costs saved through optimization.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/json-schema/cost-report.json
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
