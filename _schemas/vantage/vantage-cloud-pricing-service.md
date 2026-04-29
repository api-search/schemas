---
description: ''
layout: schema
name: Service
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
schema_file: json-schema/vantage-cloud-pricing-service-schema.json
slug: vantage-cloud-pricing-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Service.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the Service.\"\n    },\n    \"provider_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Provider this Service belongs to.\"\n    },\n    \"products_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of products available in this Service.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cloud-pricing-service-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Service
---
