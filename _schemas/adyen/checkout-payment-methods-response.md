---
description: PaymentMethodsResponse schema from Adyen API
layout: schema
name: PaymentMethodsResponse
properties_list:
- description: Detailed list of payment methods required to generate payment forms.
  name: paymentMethods
  type: array
- description: List of all stored payment methods.
  name: storedPaymentMethods
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-methods-response-schema.json
slug: checkout-payment-methods-response
source_filename: checkout-payment-methods-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-methods-response-schema.json\",\n  \"title\": \"PaymentMethodsResponse\",\n  \"description\": \"PaymentMethodsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentMethods\": {\n      \"description\": \"Detailed list of payment methods required to generate payment forms.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentMethod\"\n      },\n      \"type\": \"array\"\n    },\n    \"storedPaymentMethods\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"List of all stored payment methods.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StoredPaymentMethod\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-methods-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentMethodsResponse
---
