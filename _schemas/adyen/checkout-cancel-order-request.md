---
description: CancelOrderRequest schema from Adyen API
layout: schema
name: CancelOrderRequest
properties_list:
- description: The merchant account identifier that orderData belongs to.
  name: merchantAccount
  type: string
- description: The order request object that contains a pspReference that represents the order and the matching encrypted order data.
  name: order
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-cancel-order-request-schema.json
slug: checkout-cancel-order-request
source_filename: checkout-cancel-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-cancel-order-request-schema.json\",\n  \"title\": \"CancelOrderRequest\",\n  \"description\": \"CancelOrderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier that orderData belongs to.\",\n      \"type\": \"string\"\n    },\n    \"order\": {\n      \"description\": \"The order request object that contains a pspReference that represents the order and the matching encrypted order data.\",\n      \"$ref\": \"#/components/schemas/EncryptedOrderData\"\n    }\n  },\n  \"required\": [\n    \"order\",\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-cancel-order-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CancelOrderRequest
---
