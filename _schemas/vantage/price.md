---
description: A Price entry representing the cost of a cloud Product in a specific region and unit.
layout: schema
name: Vantage Cloud Pricing Price
properties_list:
- description: The unique identifier for the Price.
  name: id
  type: string
- description: The pricing unit (e.g., per hour, per GB-month).
  name: unit
  type: string
- description: The price amount.
  name: price
  type: string
- description: The currency of the price.
  name: currency
  type: string
- description: The cloud region this price applies to.
  name: region
  type: string
- description: A description of the pricing tier or option.
  name: description
  type: string
- description: The identifier of the associated Product.
  name: product_id
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/price.json
slug: price
source_filename: price.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/price.json\",\n  \"title\": \"Vantage Cloud Pricing Price\",\n  \"description\": \"A Price entry representing the cost of a cloud Product in a specific region and unit.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Price.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The pricing unit (e.g., per hour, per GB-month).\"\n    },\n    \"price\": {\n      \"type\": \"string\",\n      \"description\": \"The price amount.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency of the price.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud region this price applies to.\"\n    },\n    \"description\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"A description of the pricing tier or option.\"\n    },\n    \"product_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the associated Product.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/price.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Cloud Pricing Price
---
