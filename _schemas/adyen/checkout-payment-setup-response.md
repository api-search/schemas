---
description: PaymentSetupResponse schema from Adyen API
layout: schema
name: PaymentSetupResponse
properties_list:
- description: The encoded payment session that you need to pass to the SDK.
  name: paymentSession
  type: string
- description: The detailed list of stored payment details required to generate payment forms. Will be empty if oneClick is set to false in the request.
  name: recurringDetails
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-setup-response-schema.json
slug: checkout-payment-setup-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-setup-response-schema.json\",\n  \"title\": \"PaymentSetupResponse\",\n  \"description\": \"PaymentSetupResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentSession\": {\n      \"description\": \"The encoded payment session that you need to pass to the SDK.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetails\": {\n      \"deprecated\": true,\n      \"description\": \"The detailed list of stored payment details required to generate payment forms. Will be empty if oneClick is set to false in the request.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RecurringDetail\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-setup-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentSetupResponse
---
