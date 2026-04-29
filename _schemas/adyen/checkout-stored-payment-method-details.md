---
description: StoredPaymentMethodDetails schema from Adyen API
layout: schema
name: StoredPaymentMethodDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: The payment method type.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-stored-payment-method-details-schema.json
slug: checkout-stored-payment-method-details
source_filename: checkout-stored-payment-method-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-stored-payment-method-details-schema.json\",\n  \"title\": \"StoredPaymentMethodDetails\",\n  \"description\": \"StoredPaymentMethodDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This\
  \ is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The payment method type.\",\n      \"enum\": [\n        \"bcmc_mobile\",\n        \"bcmc_mobile_QR\",\n        \"bcmc_mobile_app\",\n        \"momo_wallet\",\n        \"momo_wallet_app\",\n        \"twint\",\n        \"paymaya_wallet\",\n        \"grabpay_SG\",\n        \"grabpay_MY\",\n        \"grabpay_TH\",\n        \"grabpay_ID\",\n        \"grabpay_VN\",\n        \"grabpay_PH\",\n        \"oxxo\",\n        \"gcash\",\n        \"dana\",\n        \"kakaopay\",\n        \"truemoney\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-stored-payment-method-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredPaymentMethodDetails
---
