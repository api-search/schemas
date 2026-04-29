---
description: SepaDirectDebitDetails schema from Adyen API
layout: schema
name: SepaDirectDebitDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The International Bank Account Number (IBAN).
  name: iban
  type: string
- description: The name of the bank account holder.
  name: ownerName
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: '**sepadirectdebit**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-sepa-direct-debit-details-schema.json
slug: checkout-sepa-direct-debit-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-sepa-direct-debit-details-schema.json\",\n  \"title\": \"SepaDirectDebitDetails\",\n  \"description\": \"SepaDirectDebitDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"iban\": {\n      \"description\": \"The International Bank Account Number (IBAN).\",\n      \"type\": \"string\"\n    },\n    \"ownerName\": {\n      \"description\": \"The name of the bank account holder.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\"\
  : \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"sepadirectdebit\",\n      \"description\": \"**sepadirectdebit**\",\n      \"enum\": [\n        \"sepadirectdebit\",\n        \"sepadirectdebit_amazonpay\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"iban\",\n    \"ownerName\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-sepa-direct-debit-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SepaDirectDebitDetails
---
