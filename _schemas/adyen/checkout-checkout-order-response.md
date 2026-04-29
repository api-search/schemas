---
description: CheckoutOrderResponse schema from Adyen API
layout: schema
name: CheckoutOrderResponse
properties_list:
- description: The initial amount of the order.
  name: amount
  type: object
- description: The expiry date for the order.
  name: expiresAt
  type: string
- description: The encrypted order data.
  name: orderData
  type: string
- description: The `pspReference` that belongs to the order.
  name: pspReference
  type: string
- description: The merchant reference for the order.
  name: reference
  type: string
- description: The updated remaining amount.
  name: remainingAmount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-checkout-order-response-schema.json
slug: checkout-checkout-order-response
source_filename: checkout-checkout-order-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-order-response-schema.json\",\n  \"title\": \"CheckoutOrderResponse\",\n  \"description\": \"CheckoutOrderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The initial amount of the order.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"expiresAt\": {\n      \"description\": \"The expiry date for the order.\",\n      \"type\": \"string\"\n    },\n    \"orderData\": {\n      \"description\": \"The encrypted order data.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The `pspReference` that belongs to the order.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The merchant reference for the order.\",\n      \"type\": \"string\"\
  \n    },\n    \"remainingAmount\": {\n      \"description\": \"The updated remaining amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  },\n  \"required\": [\n    \"pspReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-order-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CheckoutOrderResponse
---
