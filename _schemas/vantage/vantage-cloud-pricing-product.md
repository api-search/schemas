---
description: ''
layout: schema
name: Product
properties_list:
- description: The unique identifier for the Product.
  name: id
  type: string
- description: The display name of the Product.
  name: name
  type: string
- description: The identifier of the cloud Provider.
  name: provider_id
  type: string
- description: The identifier of the Service.
  name: service_id
  type: string
- description: Product-specific details such as vCPUs, memory, storage, network performance, etc.
  name: details
  type: object
- description: Pricing data for this Product across regions.
  name: prices
  type: array
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cloud-pricing-product-schema.json
slug: vantage-cloud-pricing-product
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Product.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the Product.\"\n    },\n    \"provider_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the cloud Provider.\"\n    },\n    \"service_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Service.\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Product-specific details such as vCPUs, memory, storage, network performance, etc.\"\n    },\n    \"prices\": {\n      \"type\": \"array\",\n      \"description\": \"Pricing data for this Product across regions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cloud-pricing-product-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Product
---
