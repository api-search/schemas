---
description: PayPalDetails schema from Adyen API
layout: schema
name: PayPalDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The unique ID associated with the order.
  name: orderID
  type: string
- description: IMMEDIATE_PAYMENT_REQUIRED or UNRESTRICTED
  name: payeePreferred
  type: string
- description: The unique ID associated with the payer.
  name: payerID
  type: string
- description: PAYPAL or PAYPAL_CREDIT
  name: payerSelected
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: The type of flow to initiate.
  name: subtype
  type: string
- description: '**paypal**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-pay-pal-details-schema.json
slug: checkout-pay-pal-details
source_filename: checkout-pay-pal-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-pay-pal-details-schema.json\",\n  \"title\": \"PayPalDetails\",\n  \"description\": \"PayPalDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"orderID\": {\n      \"description\": \"The unique ID associated with the order.\",\n      \"type\": \"string\"\n    },\n    \"payeePreferred\": {\n      \"description\": \"IMMEDIATE_PAYMENT_REQUIRED or UNRESTRICTED\",\n      \"type\": \"string\"\n    },\n    \"payerID\": {\n      \"description\": \"The unique ID associated with the payer.\",\n      \"type\": \"string\"\n    },\n    \"payerSelected\": {\n      \"description\": \"PAYPAL or PAYPAL_CREDIT\",\n      \"type\"\
  : \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"subtype\": {\n      \"description\": \"The type of flow to initiate.\",\n      \"enum\": [\n        \"redirect\",\n        \"sdk\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"paypal\",\n      \"description\": \"**paypal**\",\n      \"enum\": [\n        \"paypal\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n  \
  \  \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-pay-pal-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayPalDetails
---
