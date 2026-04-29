---
description: PaymentInstrumentUpdateRequest schema from Adyen API
layout: schema
name: PaymentInstrumentUpdateRequest
properties_list:
- description: The unique identifier of the balance account associated with this payment instrument. >You can only change the balance account ID if the payment instrument has **inactive** status.
  name: balanceAccountId
  type: string
- description: Object that contains information about the card payment instrument.
  name: card
  type: object
- description: The status of the payment instrument. If a status is not specified when creating a payment instrument, it is set to **active** by default. However, there can be exceptions for cards based on the `card
  name: status
  type: string
- description: Comment for the status of the payment instrument. Required if `statusReason` is **other**.
  name: statusComment
  type: string
- description: 'The reason for updating the status of the payment instrument. Possible values: **lost**, **stolen**, **damaged**, **suspectedFraud**, **expired**, **endOfLife**, **accountClosure**, **other**. If the '
  name: statusReason
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-payment-instrument-update-request-schema.json
slug: configuration-payment-instrument-update-request
source_filename: configuration-payment-instrument-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-payment-instrument-update-request-schema.json\",\n  \"title\": \"PaymentInstrumentUpdateRequest\",\n  \"description\": \"PaymentInstrumentUpdateRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"The unique identifier of the balance account associated with this payment instrument.\\n>You can only change the balance account ID if the payment instrument has **inactive** status.\",\n      \"type\": \"string\"\n    },\n    \"card\": {\n      \"description\": \"Object that contains information about the card payment instrument.\",\n      \"$ref\": \"#/components/schemas/CardInfo\"\n    },\n    \"status\": {\n      \"description\": \"The status of the payment instrument. If a status is not specified when creating a payment\
  \ instrument, it is set to **active** by default. However, there can be exceptions for cards based on the `card.formFactor` and the `issuingCountryCode`. For example, when issuing physical cards in the US, the default status is **inactive**.\\n\\nPossible values: \\n\\n * **active**:  The payment instrument is active and can be used to make payments. \\n\\n * **inactive**: The payment instrument is inactive and cannot be used to make payments. \\n\\n * **suspended**: The payment instrument is suspended, either because it was stolen or lost. \\n\\n * **closed**: The payment instrument is permanently closed. This action cannot be undone. \\n\\n\",\n      \"enum\": [\n        \"active\",\n        \"closed\",\n        \"inactive\",\n        \"suspended\"\n      ],\n      \"type\": \"string\"\n    },\n    \"statusComment\": {\n      \"description\": \"Comment for the status of the payment instrument.\\n\\nRequired if `statusReason` is **other**.\",\n      \"type\": \"string\"\n    },\n    \"\
  statusReason\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The reason for updating the status of the payment instrument.\\n\\nPossible values: **lost**, **stolen**, **damaged**, **suspectedFraud**, **expired**, **endOfLife**, **accountClosure**, **other**.\\nIf the reason is **other**, you must also send the `statusComment` parameter describing the status change.\",\n      \"enum\": [\n        \"accountClosure\",\n        \"damaged\",\n        \"endOfLife\",\n        \"expired\",\n        \"lost\",\n        \"other\",\n        \"stolen\",\n        \"suspectedFraud\",\n        \"transactionRule\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-payment-instrument-update-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrumentUpdateRequest
---
