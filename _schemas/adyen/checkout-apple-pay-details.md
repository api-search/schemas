---
description: ApplePayDetails schema from Adyen API
layout: schema
name: ApplePayDetails
properties_list:
- description: The stringified and base64 encoded `paymentData` you retrieved from the Apple framework.
  name: applePayToken
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The funding source that should be used when multiple sources are available. For Brazilian combo cards, by default the funding source is credit. To use debit, set this value to **debit**.
  name: fundingSource
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: '**applepay**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-apple-pay-details-schema.json
slug: checkout-apple-pay-details
source_filename: checkout-apple-pay-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-apple-pay-details-schema.json\",\n  \"title\": \"ApplePayDetails\",\n  \"description\": \"ApplePayDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applePayToken\": {\n      \"description\": \"The stringified and base64 encoded `paymentData` you retrieved from the Apple framework.\",\n      \"maxLength\": 10000,\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"fundingSource\": {\n      \"description\": \"The funding source that should be used when multiple sources are available. For Brazilian combo cards, by default the funding source is credit. To use debit, set this value to **debit**.\",\n      \"enum\": [\n\
  \        \"credit\",\n        \"debit\"\n      ],\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"applepay\",\n      \"description\": \"**applepay**\",\n      \"enum\": [\n        \"applepay\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"applePayToken\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-apple-pay-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ApplePayDetails
---
