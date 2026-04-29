---
description: PaymentInstrument schema from Adyen API
layout: schema
name: PaymentInstrument
properties_list:
- description: The unique identifier of the [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/v1/post/balanceAccounts__resParam_id) associated with the payment instrument.
  name: balanceAccountId
  type: string
- description: Contains the business account details. Returned when you create a payment instrument with `type` **bankAccount**.
  name: bankAccount
  type: object
- description: Contains information about the card payment instrument. Returned when you create a payment instrument with `type` **card**.
  name: card
  type: object
- description: Your description for the payment instrument, maximum 300 characters.
  name: description
  type: string
- description: The unique identifier of the payment instrument.
  name: id
  type: string
- description: The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code where the payment instrument is issued. For example, **NL** or **US**.
  name: issuingCountryCode
  type: string
- description: The unique identifier of the [payment instrument group](https://docs.adyen.com/api-explorer/#/balanceplatform/v1/post/paymentInstrumentGroups__resParam_id) to which the payment instrument belongs.
  name: paymentInstrumentGroupId
  type: string
- description: Your reference for the payment instrument, maximum 150 characters.
  name: reference
  type: string
- description: The status of the payment instrument. If a status is not specified when creating a payment instrument, it is set to **Active** by default. However, there can be exceptions for cards based on the `card
  name: status
  type: string
- description: 'Type of payment instrument. Possible value: **card**, **bankAccount**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-payment-instrument-schema.json
slug: configuration-webhooks-payment-instrument
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-payment-instrument-schema.json\",\n  \"title\": \"PaymentInstrument\",\n  \"description\": \"PaymentInstrument schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"The unique identifier of the [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/v1/post/balanceAccounts__resParam_id) associated with the payment instrument.\",\n      \"type\": \"string\"\n    },\n    \"bankAccount\": {\n      \"description\": \"Contains the business account details. Returned when you create a payment instrument with `type` **bankAccount**.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IbanAccountIdentification\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/USLocalAccountIdentification\"\
  \n        }\n      ]\n    },\n    \"card\": {\n      \"description\": \"Contains information about the card payment instrument. Returned when you create a payment instrument with `type` **card**.\",\n      \"$ref\": \"#/components/schemas/Card\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the payment instrument, maximum 300 characters.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the payment instrument.\",\n      \"type\": \"string\"\n    },\n    \"issuingCountryCode\": {\n      \"description\": \"The two-character [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) country code where the payment instrument is issued. For example, **NL** or **US**.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrumentGroupId\": {\n      \"description\": \"The unique identifier of the [payment instrument group](https://docs.adyen.com/api-explorer/#/balanceplatform/v1/post/paymentInstrumentGroups__resParam_id)\
  \ to which the payment instrument belongs.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the payment instrument, maximum 150 characters.\",\n      \"maxLength\": 150,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the payment instrument. If a status is not specified when creating a payment instrument, it is set to **Active** by default. However, there can be exceptions for cards based on the `card.formFactor` and the `issuingCountryCode`. For example, when issuing physical cards in the US, the default status is **Requested**.\\n\\nPossible values: \\n\\n * **Active**:  The payment instrument is active and can be used to make payments. \\n\\n * **Requested**: The payment instrument has been requested. This state is applicable for physical cards. \\n\\n* **Inactive**: The payment instrument is inactive and cannot be used to make payments. \\n\\n * **Suspended**: The payment instrument\
  \ is temporarily suspended and cannot be used to make payments. \\n\\n * **Closed**: The payment instrument is permanently closed. This action cannot be undone. \\n\\n* **Stolen** \\n\\n * **Lost**\\n\\n \",\n      \"enum\": [\n        \"Active\",\n        \"Closed\",\n        \"Inactive\",\n        \"Lost\",\n        \"Requested\",\n        \"Stolen\",\n        \"Suspended\",\n        \"blocked\",\n        \"discarded\"\n      ],\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type of payment instrument.\\n\\nPossible value: **card**, **bankAccount**. \",\n      \"enum\": [\n        \"bankAccount\",\n        \"card\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"balanceAccountId\",\n    \"issuingCountryCode\",\n    \"type\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-payment-instrument-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrument
---
