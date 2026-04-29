---
description: GenericIssuerPaymentMethodDetails schema from Adyen API
layout: schema
name: GenericIssuerPaymentMethodDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The issuer id of the shopper's selected bank.
  name: issuer
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: '**genericissuer**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-generic-issuer-payment-method-details-schema.json
slug: checkout-generic-issuer-payment-method-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-generic-issuer-payment-method-details-schema.json\",\n  \"title\": \"GenericIssuerPaymentMethodDetails\",\n  \"description\": \"GenericIssuerPaymentMethodDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"description\": \"The issuer id of the shopper's selected bank.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created\
  \ the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**genericissuer**\",\n      \"enum\": [\n        \"onlineBanking_PL\",\n        \"eps\",\n        \"onlineBanking_SK\",\n        \"onlineBanking_CZ\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"issuer\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-generic-issuer-payment-method-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GenericIssuerPaymentMethodDetails
---
