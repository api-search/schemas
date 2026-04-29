---
description: BacsDirectDebitDetails schema from Adyen API
layout: schema
name: BacsDirectDebitDetails
properties_list:
- description: The bank account number (without separators).
  name: bankAccountNumber
  type: string
- description: The bank routing number of the account.
  name: bankLocationId
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The name of the bank account holder.
  name: holderName
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: '**directdebit_GB**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-bacs-direct-debit-details-schema.json
slug: checkout-bacs-direct-debit-details
source_filename: checkout-bacs-direct-debit-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-bacs-direct-debit-details-schema.json\",\n  \"title\": \"BacsDirectDebitDetails\",\n  \"description\": \"BacsDirectDebitDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccountNumber\": {\n      \"x-addedInVersion\": \"65\",\n      \"description\": \"The bank account number (without separators).\",\n      \"type\": \"string\"\n    },\n    \"bankLocationId\": {\n      \"x-addedInVersion\": \"65\",\n      \"description\": \"The bank routing number of the account.\",\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"holderName\": {\n      \"x-addedInVersion\": \"65\",\n      \"description\": \"The name of the bank\
  \ account holder.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"directdebit_GB\",\n      \"description\": \"**directdebit_GB**\",\n      \"enum\": [\n        \"directdebit_GB\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-bacs-direct-debit-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BacsDirectDebitDetails
---
