---
description: OrderItem schema from Adyen API
layout: schema
name: OrderItem
properties_list:
- description: The unique identifier of the product.
  name: id
  type: string
- description: The number of installments for the specified product `id`.
  name: installments
  type: integer
- description: The name of the product.
  name: name
  type: string
- description: The number of items with the specified product `id` included in the order.
  name: quantity
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-order-item-schema.json
slug: management-order-item
source_filename: management-order-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-order-item-schema.json\",\n  \"title\": \"OrderItem\",\n  \"description\": \"OrderItem schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The unique identifier of the product.\",\n      \"type\": \"string\"\n    },\n    \"installments\": {\n      \"description\": \"The number of installments for the specified product `id`.\",\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"description\": \"The name of the product.\",\n      \"type\": \"string\"\n    },\n    \"quantity\": {\n      \"description\": \"The number of items with the specified product `id` included in the order.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-order-item-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OrderItem
---
