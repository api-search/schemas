---
description: ''
layout: schema
name: CommitmentPlan
properties_list:
- description: The unique identifier of the commitment plan.
  name: id
  type: string
- description: The type of commitment.
  name: type
  type: string
- description: The cloud provider.
  name: provider
  type: string
- description: The current status of the commitment plan.
  name: status
  type: string
- description: The start date of the commitment.
  name: startDate
  type: string
- description: The end date of the commitment.
  name: endDate
  type: string
- description: Estimated monthly savings from this commitment.
  name: monthlySavings
  type: number
- description: Current utilization percentage of the commitment.
  name: utilizationPercentage
  type: number
provider_name: Spot
provider_slug: spot
schema_file: json-schema/spot-eco-commitment-plan-schema.json
slug: spot-eco-commitment-plan
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CommitmentPlan\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the commitment plan.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of commitment.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the commitment plan.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The start date of the commitment.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"The end date of the commitment.\"\n    },\n    \"monthlySavings\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated monthly savings from this commitment.\"\n   \
  \ },\n    \"utilizationPercentage\": {\n      \"type\": \"number\",\n      \"description\": \"Current utilization percentage of the commitment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/spot-eco-commitment-plan-schema.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: CommitmentPlan
---
