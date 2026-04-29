---
description: DonationPaymentResponse schema from Adyen API
layout: schema
name: DonationPaymentResponse
properties_list:
- description: Authorised amount in the transaction.
  name: amount
  type: object
- description: The Adyen account name of your charity. We will provide you with this account name once your chosen charity has been [onboarded](https://docs.adyen.com/online-payments/donations#onboarding).
  name: donationAccount
  type: string
- description: Your unique resource identifier.
  name: id
  type: string
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: Action to be taken for completing the payment.
  name: payment
  type: object
- description: The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a require
  name: reference
  type: string
- description: 'The status of the donation transaction. Possible values: * **completed** * **pending** * **refused**'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-donation-payment-response-schema.json
slug: checkout-donation-payment-response
source_filename: checkout-donation-payment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-donation-payment-response-schema.json\",\n  \"title\": \"DonationPaymentResponse\",\n  \"description\": \"DonationPaymentResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"Authorised amount in the transaction.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"donationAccount\": {\n      \"description\": \"The Adyen account name of your charity. We will provide you with this account name once your chosen charity has been [onboarded](https://docs.adyen.com/online-payments/donations#onboarding).\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"Your unique resource identifier.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account\
  \ identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"payment\": {\n      \"description\": \"Action to be taken for completing the payment.\",\n      \"$ref\": \"#/components/schemas/PaymentResponse\"\n    },\n    \"reference\": {\n      \"description\": \"The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a requirement. If you need to provide multiple references for a transaction, separate them with hyphens (\\\"-\\\"). Maximum length: 80 characters.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the donation transaction.\\n\\nPossible values:\\n* **completed**\\n* **pending**\\n* **refused**\",\n      \"enum\": [\n        \"completed\",\n        \"pending\",\n        \"refused\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-donation-payment-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DonationPaymentResponse
---
