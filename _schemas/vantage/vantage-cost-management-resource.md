---
description: ''
layout: schema
name: Resource
properties_list:
- description: The unique identifier for the Resource.
  name: token
  type: string
- description: The name of the Resource.
  name: name
  type: string
- description: The cloud provider.
  name: provider
  type: string
- description: The cloud service.
  name: service
  type: string
- description: The cloud account identifier.
  name: account_id
  type: string
- description: The region of the resource.
  name: region
  type: string
- description: The cost associated with the resource.
  name: cost
  type: string
- description: Additional metadata about the resource.
  name: metadata
  type: object
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-resource-schema.json
slug: vantage-cost-management-resource
source_filename: vantage-cost-management-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Resource.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Resource.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider.\"\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud service.\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud account identifier.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The region of the resource.\"\n    },\n    \"cost\": {\n      \"type\": \"string\",\n      \"description\": \"The cost associated with the resource.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n  \
  \    \"description\": \"Additional metadata about the resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-resource-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Resource
---
