---
description: ''
layout: schema
name: BillingAccount
properties_list:
- description: The Spot account identifier.
  name: accountId
  type: string
- description: The cloud provider type.
  name: cloudProvider
  type: string
- description: The setup status of the billing account.
  name: status
  type: string
- description: The cloud provider billing account identifier.
  name: billingAccountId
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/spot-billing-engine-billing-account-schema.json
slug: spot-billing-engine-billing-account
source_filename: spot-billing-engine-billing-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BillingAccount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The Spot account identifier.\"\n    },\n    \"cloudProvider\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider type.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The setup status of the billing account.\"\n    },\n    \"billingAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider billing account identifier.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/spot-billing-engine-billing-account-schema.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: BillingAccount
---
