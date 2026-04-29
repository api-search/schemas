---
description: PaymentVerificationRequest schema from Adyen API
layout: schema
name: PaymentVerificationRequest
properties_list:
- description: Encrypted and signed payment result data. You should receive this value from the Checkout SDK after the shopper completes the payment.
  name: payload
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-verification-request-schema.json
slug: checkout-payment-verification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-verification-request-schema.json\",\n  \"title\": \"PaymentVerificationRequest\",\n  \"description\": \"PaymentVerificationRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"payload\": {\n      \"description\": \"Encrypted and signed payment result data. You should receive this value from the Checkout SDK after the shopper completes the payment.\",\n      \"maxLength\": 40000,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"payload\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-verification-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentVerificationRequest
---
