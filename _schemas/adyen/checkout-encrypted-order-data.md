---
description: EncryptedOrderData schema from Adyen API
layout: schema
name: EncryptedOrderData
properties_list:
- description: The encrypted order data.
  name: orderData
  type: string
- description: The `pspReference` that belongs to the order.
  name: pspReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-encrypted-order-data-schema.json
slug: checkout-encrypted-order-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-encrypted-order-data-schema.json\",\n  \"title\": \"EncryptedOrderData\",\n  \"description\": \"EncryptedOrderData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderData\": {\n      \"description\": \"The encrypted order data.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The `pspReference` that belongs to the order.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pspReference\",\n    \"orderData\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-encrypted-order-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EncryptedOrderData
---
