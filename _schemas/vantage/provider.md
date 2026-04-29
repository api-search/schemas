---
description: A cloud Provider with pricing data available in the Vantage Cloud Pricing API.
layout: schema
name: Vantage Cloud Pricing Provider
properties_list:
- description: The unique identifier for the Provider.
  name: id
  type: string
- description: The display name of the Provider.
  name: name
  type: string
- description: The number of services available from this Provider.
  name: services_count
  type: integer
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/provider.json
slug: provider
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/provider.json\",\n  \"title\": \"Vantage Cloud Pricing Provider\",\n  \"description\": \"A cloud Provider with pricing data available in the Vantage Cloud Pricing API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Provider.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the Provider.\"\n    },\n    \"services_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of services available from this Provider.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/provider.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Cloud Pricing Provider
---
