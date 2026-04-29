---
description: PaymentAmountUpdateRequest schema from Adyen API
layout: schema
name: PaymentAmountUpdateRequest
properties_list:
- description: The updated amount. The `currency` must match the currency used in authorisation.
  name: amount
  type: object
- description: Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).
  name: applicationInfo
  type: object
- description: 'The reason for the amount update. Possible values: * **delayedCharge** * **noShow** * **installment**'
  name: industryUsage
  type: string
- description: Price and product information of the refunded items, required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment). > This field is required for partial refunds with 3
  name: lineItems
  type: array
- description: The merchant account that is used to process the payment.
  name: merchantAccount
  type: string
- description: 'Your reference for the amount update request. Maximum length: 80 characters.'
  name: reference
  type: string
- description: An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-a
  name: splits
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-amount-update-request-schema.json
slug: checkout-payment-amount-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-amount-update-request-schema.json\",\n  \"title\": \"PaymentAmountUpdateRequest\",\n  \"description\": \"PaymentAmountUpdateRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The updated amount. The `currency` must match the currency used in authorisation.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"applicationInfo\": {\n      \"description\": \"Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).\",\n      \"$ref\": \"#/components/schemas/ApplicationInfo\"\n    },\n    \"industryUsage\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"The reason for the amount update. Possible values:\
  \ \\n* **delayedCharge** \\n* **noShow** \\n* **installment**\",\n      \"enum\": [\n        \"delayedCharge\",\n        \"installment\",\n        \"noShow\"\n      ],\n      \"type\": \"string\"\n    },\n    \"lineItems\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Price and product information of the refunded items, required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment).\\n> This field is required for partial refunds with 3x 4x Oney, Affirm, Afterpay, Atome, Clearpay, Klarna, Ratepay, Walley, and Zip.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the amount update request. Maximum length: 80 characters.\",\n      \"type\": \"string\"\n\
  \    },\n    \"splits\": {\n      \"description\": \"An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-amount-update-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentAmountUpdateRequest
---
