---
description: A cloud Service within a Provider, containing products with pricing data.
layout: schema
name: Vantage Cloud Pricing Service
properties_list:
- description: The unique identifier for the Service.
  name: id
  type: string
- description: The display name of the Service.
  name: name
  type: string
- description: The identifier of the Provider this Service belongs to.
  name: provider_id
  type: string
- description: The number of products available in this Service.
  name: products_count
  type: integer
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/service.json
slug: service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/service.json\",\n  \"title\": \"Vantage Cloud Pricing Service\",\n  \"description\": \"A cloud Service within a Provider, containing products with pricing data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Service.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the Service.\"\n    },\n    \"provider_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Provider this Service belongs to.\"\n    },\n    \"products_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of products available in this Service.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/service.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Cloud Pricing Service
---
