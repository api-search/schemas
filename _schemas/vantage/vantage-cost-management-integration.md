---
description: ''
layout: schema
name: Integration
properties_list:
- description: The unique token identifier for the Integration.
  name: token
  type: string
- description: The cloud provider (e.g., aws, azure, gcp).
  name: provider
  type: string
- description: The current status of the Integration.
  name: status
  type: string
- description: The cloud account identifier for the Integration.
  name: account_identifier
  type: string
- description: The date and time the Integration was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-integration-schema.json
slug: vantage-cost-management-integration
source_filename: vantage-cost-management-integration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Integration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Integration.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider (e.g., aws, azure, gcp).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the Integration.\"\n    },\n    \"account_identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud account identifier for the Integration.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the Integration was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-integration-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Integration
---
