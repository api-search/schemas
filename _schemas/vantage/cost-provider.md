---
description: A Cost Provider representing a cloud or SaaS provider whose cost data is available in Vantage.
layout: schema
name: Vantage Cost Provider
properties_list:
- description: The unique token identifier for the Cost Provider.
  name: token
  type: string
- description: The name of the Cost Provider.
  name: name
  type: string
- description: A description of the Cost Provider.
  name: description
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/cost-provider.json
slug: cost-provider
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/cost-provider.json\",\n  \"title\": \"Vantage Cost Provider\",\n  \"description\": \"A Cost Provider representing a cloud or SaaS provider whose cost data is available in Vantage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Cost Provider.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Cost Provider.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the Cost Provider.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/cost-provider.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Cost Provider
---
