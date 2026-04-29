---
description: AfterpayDetails schema from Adyen API
layout: schema
name: AfterpayDetails
properties_list:
- description: The address where to send the invoice.
  name: billingAddress
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The address where the goods should be delivered.
  name: deliveryAddress
  type: string
- description: Shopper name, date of birth, phone number, and email address.
  name: personalDetails
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: '**afterpay_default**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-afterpay-details-schema.json
slug: checkout-afterpay-details
source_filename: checkout-afterpay-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-afterpay-details-schema.json\",\n  \"title\": \"AfterpayDetails\",\n  \"description\": \"AfterpayDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingAddress\": {\n      \"description\": \"The address where to send the invoice.\",\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"deliveryAddress\": {\n      \"description\": \"The address where the goods should be delivered.\",\n      \"type\": \"string\"\n    },\n    \"personalDetails\": {\n      \"description\": \"Shopper name, date of birth, phone number, and email address.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"\
  deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"afterpay_default\",\n      \"description\": \"**afterpay_default**\",\n      \"enum\": [\n        \"afterpay_default\",\n        \"afterpaytouch\",\n        \"afterpay_b2b\",\n        \"clearpay\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-afterpay-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AfterpayDetails
---
