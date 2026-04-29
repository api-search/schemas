---
description: ResponsePaymentMethod schema from Adyen API
layout: schema
name: ResponsePaymentMethod
properties_list:
- description: The card brand that the shopper used to pay. Only returned if `paymentMethod.type` is **scheme**.
  name: brand
  type: string
- description: The `paymentMethod.type` value used in the request.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-response-payment-method-schema.json
slug: checkout-response-payment-method
source_filename: checkout-response-payment-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-response-payment-method-schema.json\",\n  \"title\": \"ResponsePaymentMethod\",\n  \"description\": \"ResponsePaymentMethod schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"description\": \"The card brand that the shopper used to pay. Only returned if `paymentMethod.type` is **scheme**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The `paymentMethod.type` value used in the request.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-response-payment-method-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponsePaymentMethod
---
