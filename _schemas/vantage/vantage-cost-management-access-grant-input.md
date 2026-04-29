---
description: ''
layout: schema
name: AccessGrantInput
properties_list:
- description: The token of the Team to grant access to.
  name: team_token
  type: string
- description: The token of the resource to grant access to.
  name: resource_token
  type: string
- description: The level of access to grant.
  name: access
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-access-grant-input-schema.json
slug: vantage-cost-management-access-grant-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessGrantInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"team_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Team to grant access to.\"\n    },\n    \"resource_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the resource to grant access to.\"\n    },\n    \"access\": {\n      \"type\": \"string\",\n      \"description\": \"The level of access to grant.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-access-grant-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: AccessGrantInput
---
