---
description: A cloud cost record representing spending from a cloud service provider (AWS, Azure, or GCP), aggregated by account, service, provider, or label.
layout: schema
name: Kubecost Cloud Cost
properties_list:
- description: Invoice entity identifier from the cloud provider.
  name: invoiceEntityID
  type: string
- description: Cloud provider account identifier.
  name: accountID
  type: string
- description: Cloud service provider name (e.g. AWS, Azure, GCP).
  name: provider
  type: string
- description: Cloud provider service name.
  name: service
  type: string
- description: Labels associated with the cloud cost item.
  name: labels
  type: object
- description: The time window for this cloud cost record.
  name: window
  type: object
- description: List price cost before discounts.
  name: listCost
  type: number
- description: Net cost after discounts and credits.
  name: netCost
  type: number
- description: Amortized net cost spreading upfront payments over time.
  name: amortizedNetCost
  type: number
- description: Invoiced cost from the cloud provider.
  name: invoicedCost
  type: number
provider_name: Kubecost
provider_slug: kubecost
schema_file: json-schema/cloud-cost.json
slug: cloud-cost
source_filename: cloud-cost.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/kubecost/blob/main/json-schema/cloud-cost.json\",\n  \"title\": \"Kubecost Cloud Cost\",\n  \"description\": \"A cloud cost record representing spending from a cloud service provider (AWS, Azure, or GCP), aggregated by account, service, provider, or label.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceEntityID\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice entity identifier from the cloud provider.\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider account identifier.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud service provider name (e.g. AWS, Azure, GCP).\"\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider service name.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n\
  \      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels associated with the cloud cost item.\"\n    },\n    \"window\": {\n      \"type\": \"object\",\n      \"description\": \"The time window for this cloud cost record.\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Start of the window.\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"End of the window.\"\n        }\n      }\n    },\n    \"listCost\": {\n      \"type\": \"number\",\n      \"description\": \"List price cost before discounts.\"\n    },\n    \"netCost\": {\n      \"type\": \"number\",\n      \"description\": \"Net cost after discounts and credits.\"\n    },\n    \"amortizedNetCost\": {\n      \"type\": \"number\",\n      \"description\": \"Amortized net cost spreading upfront payments\
  \ over time.\"\n    },\n    \"invoicedCost\": {\n      \"type\": \"number\",\n      \"description\": \"Invoiced cost from the cloud provider.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/json-schema/cloud-cost.json
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
title: Kubecost Cloud Cost
---
