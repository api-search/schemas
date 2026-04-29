---
description: A Kubernetes Efficiency Report measuring cluster and namespace cost efficiency, idle costs, and total costs.
layout: schema
name: Vantage Kubernetes Efficiency Report
properties_list:
- description: The unique token identifier for the report.
  name: token
  type: string
- description: The Kubernetes cluster name.
  name: cluster_name
  type: string
- description: The Kubernetes namespace.
  name: namespace
  type: string
- description: The idle cost for the cluster/namespace.
  name: idle_cost
  type: string
- description: The total cost for the cluster/namespace.
  name: total_cost
  type: string
- description: The efficiency percentage.
  name: efficiency
  type: number
- description: The date and time the report was generated.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/kubernetes-efficiency-report.json
slug: kubernetes-efficiency-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/kubernetes-efficiency-report.json\",\n  \"title\": \"Vantage Kubernetes Efficiency Report\",\n  \"description\": \"A Kubernetes Efficiency Report measuring cluster and namespace cost efficiency, idle costs, and total costs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the report.\"\n    },\n    \"cluster_name\": {\n      \"type\": \"string\",\n      \"description\": \"The Kubernetes cluster name.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The Kubernetes namespace.\"\n    },\n    \"idle_cost\": {\n      \"type\": \"string\",\n      \"description\": \"The idle cost for the cluster/namespace.\"\n    },\n    \"total_cost\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ total cost for the cluster/namespace.\"\n    },\n    \"efficiency\": {\n      \"type\": \"number\",\n      \"description\": \"The efficiency percentage.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the report was generated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/kubernetes-efficiency-report.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Kubernetes Efficiency Report
---
