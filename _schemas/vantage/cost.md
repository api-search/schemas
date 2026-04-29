---
description: A cost data entry representing cloud spending for a specific date, provider, service, and account.
layout: schema
name: Vantage Cost
properties_list:
- description: The date of the cost entry.
  name: date
  type: string
- description: The cost amount.
  name: amount
  type: string
- description: The currency of the cost amount.
  name: currency
  type: string
- description: The cloud provider (e.g., aws, azure, gcp).
  name: provider
  type: string
- description: The cloud service name.
  name: service
  type: string
- description: The cloud account identifier.
  name: account_id
  type: string
- description: The cloud region.
  name: region
  type: string
- description: The cost category.
  name: category
  type: string
- description: The cost subcategory.
  name: subcategory
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/cost.json
slug: cost
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/cost.json\",\n  \"title\": \"Vantage Cost\",\n  \"description\": \"A cost data entry representing cloud spending for a specific date, provider, service, and account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the cost entry.\"\n    },\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"The cost amount.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency of the cost amount.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider (e.g., aws, azure, gcp).\"\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud service name.\"\n    },\n    \"account_id\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"The cloud account identifier.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud region.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The cost category.\"\n    },\n    \"subcategory\": {\n      \"type\": \"string\",\n      \"description\": \"The cost subcategory.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/cost.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Cost
---
