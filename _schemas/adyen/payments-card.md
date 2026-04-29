---
description: Card schema from Adyen API
layout: schema
name: Card
properties_list:
- description: 'The [card verification code](https://docs.adyen.com/payments-fundamentals/payment-glossary#card-security-code-cvc-cvv-cid) (1-20 characters). Depending on the card brand, it is known also as: * CVV2/C'
  name: cvc
  type: string
- description: 'The card expiry month. Format: 2 digits, zero-padded for single digits. For example: * 03 = March * 11 = November'
  name: expiryMonth
  type: string
- description: 'The card expiry year. Format: 4 digits. For example: 2020'
  name: expiryYear
  type: string
- description: The name of the cardholder, as printed on the card.
  name: holderName
  type: string
- description: The issue number of the card (for some UK debit cards only).
  name: issueNumber
  type: string
- description: The card number (4-19 characters). Do not use any separators. When this value is returned in a response, only the last 4 digits of the card number are returned.
  name: number
  type: string
- description: The month component of the start date (for some UK debit cards only).
  name: startMonth
  type: string
- description: The year component of the start date (for some UK debit cards only).
  name: startYear
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-card-schema.json
slug: payments-card
source_filename: payments-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-card-schema.json\",\n  \"title\": \"Card\",\n  \"description\": \"Card schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cvc\": {\n      \"description\": \"The [card verification code](https://docs.adyen.com/payments-fundamentals/payment-glossary#card-security-code-cvc-cvv-cid) (1-20 characters). Depending on the card brand, it is known also as:\\n* CVV2/CVC2 \\u2013 length: 3 digits\\n* CID \\u2013 length: 4 digits\\n> If you are using [Client-Side Encryption](https://docs.adyen.com/classic-integration/cse-integration-ecommerce), the CVC code is present in the encrypted data. You must never post the card details to the server.\\n> This field must be always present in a [one-click payment request](https://docs.adyen.com/classic-integration/recurring-payments).\\n> When this value\
  \ is returned in a response, it is always empty because it is not stored.\",\n      \"maxLength\": 20,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"expiryMonth\": {\n      \"description\": \"The card expiry month.\\nFormat: 2 digits, zero-padded for single digits. For example:\\n* 03 = March\\n* 11 = November\",\n      \"maxLength\": 2,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"expiryYear\": {\n      \"description\": \"The card expiry year.\\nFormat: 4 digits. For example: 2020\",\n      \"maxLength\": 4,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"holderName\": {\n      \"description\": \"The name of the cardholder, as printed on the card.\",\n      \"maxLength\": 50,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"issueNumber\": {\n      \"description\": \"The issue number of the card (for some UK debit cards only).\",\n      \"maxLength\": 2,\n      \"minLength\": 1,\n      \"type\": \"string\"\
  \n    },\n    \"number\": {\n      \"description\": \"The card number (4-19 characters). Do not use any separators.\\nWhen this value is returned in a response, only the last 4 digits of the card number are returned.\",\n      \"maxLength\": 19,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    },\n    \"startMonth\": {\n      \"description\": \"The month component of the start date (for some UK debit cards only).\",\n      \"maxLength\": 2,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"startYear\": {\n      \"description\": \"The year component of the start date (for some UK debit cards only).\",\n      \"maxLength\": 4,\n      \"minLength\": 4,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-card-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Card
---
