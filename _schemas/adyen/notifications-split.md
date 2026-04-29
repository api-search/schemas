---
description: Split schema from Adyen API
layout: schema
name: Split
properties_list:
- description: Unique identifier of the account where the split amount should be sent. This is required if `type` is **MarketPlace** or **BalanceAccount**.
  name: account
  type: string
- description: The amount of this split.
  name: amount
  type: object
- description: A description of this split.
  name: description
  type: string
- description: Your reference for the split, which you can use to link the split to other operations such as captures and refunds. This is required if `type` is **MarketPlace** or **BalanceAccount**. For the other t
  name: reference
  type: string
- description: 'The type of split. Possible values: **Default**, **PaymentFee**, **VAT**, **Commission**, **MarketPlace**, **BalanceAccount**, **Remainder**, **Surcharge**, **Tip**.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-split-schema.json
slug: notifications-split
source_filename: notifications-split-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-split-schema.json\",\n  \"title\": \"Split\",\n  \"description\": \"Split schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account\": {\n      \"description\": \"Unique identifier of the account where the split amount should be sent. This is required if `type` is **MarketPlace** or **BalanceAccount**.\\n\\n\",\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"description\": \"The amount of this split.\",\n      \"$ref\": \"#/components/schemas/SplitAmount\"\n    },\n    \"description\": {\n      \"description\": \"A description of this split.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the split, which you can use to link the split to other operations such as captures and refunds.\\n\\nThis is required\
  \ if `type` is **MarketPlace** or **BalanceAccount**. For the other types, we also recommend sending a reference so you can reconcile the split and the associated payment in the transaction overview and in the reports. If the reference is not provided, the split is reported as part of the aggregated [TransferBalance record type](https://docs.adyen.com/reporting/marketpay-payments-accounting-report) in Adyen for Platforms.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of split.\\nPossible values: **Default**, **PaymentFee**, **VAT**, **Commission**, **MarketPlace**, **BalanceAccount**, **Remainder**, **Surcharge**, **Tip**.\",\n      \"enum\": [\n        \"BalanceAccount\",\n        \"Commission\",\n        \"Default\",\n        \"MarketPlace\",\n        \"PaymentFee\",\n        \"PaymentFeeAcquiring\",\n        \"PaymentFeeAdyen\",\n        \"PaymentFeeAdyenCommission\",\n        \"PaymentFeeAdyenMarkup\",\n        \"PaymentFeeInterchange\"\
  ,\n        \"PaymentFeeSchemeFee\",\n        \"Remainder\",\n        \"Surcharge\",\n        \"Tip\",\n        \"VAT\",\n        \"Verification\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-split-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Split
---
