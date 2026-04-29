---
description: CreateOrderRequest schema from Adyen API
layout: schema
name: CreateOrderRequest
properties_list:
- description: The total amount of the order.
  name: amount
  type: object
- description: The date that order expires; e.g. 2019-03-23T12:25:28Z. If not provided, the default expiry duration is 1 day.
  name: expiresAt
  type: string
- description: The merchant account identifier, with which you want to process the order.
  name: merchantAccount
  type: string
- description: A custom reference identifying the order.
  name: reference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-create-order-request-schema.json
slug: checkout-create-order-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-create-order-request-schema.json\",\n  \"title\": \"CreateOrderRequest\",\n  \"description\": \"CreateOrderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The total amount of the order.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"expiresAt\": {\n      \"description\": \"The date that order expires; e.g. 2019-03-23T12:25:28Z. If not provided, the default expiry duration is 1 day.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the order.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"A custom reference identifying the order.\",\n      \"type\": \"string\"\n   \
  \ }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"reference\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-create-order-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateOrderRequest
---
