---
description: Request body for creating a new order
layout: schema
name: CreateOrderRequest
properties_list:
- description: Line items to order
  name: items
  type: array
- description: ''
  name: shippingAddress
  type: object
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-create-order-request-schema.json
slug: 3m-partner-supplier-api-create-order-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-create-order-request-schema.json\",\n  \"title\": \"CreateOrderRequest\",\n  \"description\": \"Request body for creating a new order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Line items to order\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"productId\": {\n            \"type\": \"string\",\n            \"description\": \"Product identifier\",\n            \"example\": \"PROD-12345\"\n          },\n          \"quantity\": {\n            \"type\": \"integer\",\n            \"description\": \"Quantity to order\",\n            \"example\": 20\n          }\n        }\n      }\n    },\n    \"shippingAddress\": {\n      \"$ref\": \"#/components/schemas/ShippingAddress\"\n\
  \    }\n  },\n  \"required\": [\n    \"items\",\n    \"shippingAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-create-order-request-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: CreateOrderRequest
---
