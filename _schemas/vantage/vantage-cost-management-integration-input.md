---
description: ''
layout: schema
name: IntegrationInput
properties_list:
- description: The cloud provider to integrate with.
  name: provider
  type: string
- description: The cloud account identifier.
  name: account_identifier
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-integration-input-schema.json
slug: vantage-cost-management-integration-input
source_filename: vantage-cost-management-integration-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntegrationInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider to integrate with.\"\n    },\n    \"account_identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud account identifier.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-integration-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: IntegrationInput
---
