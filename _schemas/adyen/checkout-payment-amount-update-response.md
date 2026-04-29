---
description: PaymentAmountUpdateResponse schema from Adyen API
layout: schema
name: PaymentAmountUpdateResponse
properties_list:
- description: The updated amount.
  name: amount
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
- description: The [`pspReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_pspReference) of the payment to update.
  name: paymentPspReference
  type: string
- description: Adyen's 16-character reference associated with the amount update request.
  name: pspReference
  type: string
- description: 'Your reference for the amount update request. Maximum length: 80 characters.'
  name: reference
  type: string
- description: An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-a
  name: splits
  type: array
- description: The status of your request. This will always have the value **received**.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-amount-update-response-schema.json
slug: checkout-payment-amount-update-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-amount-update-response-schema.json\",\n  \"title\": \"PaymentAmountUpdateResponse\",\n  \"description\": \"PaymentAmountUpdateResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The updated amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"industryUsage\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"The reason for the amount update. Possible values: \\n* **delayedCharge** \\n* **noShow** \\n* **installment**\",\n      \"enum\": [\n        \"delayedCharge\",\n        \"installment\",\n        \"noShow\"\n      ],\n      \"type\": \"string\"\n    },\n    \"lineItems\": {\n      \"x-addedInVersion\": \"71\",\n      \"description\": \"Price and product information of the refunded items,\
  \ required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment).\\n> This field is required for partial refunds with 3x 4x Oney, Affirm, Afterpay, Atome, Clearpay, Klarna, Ratepay, Walley, and Zip.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"paymentPspReference\": {\n      \"description\": \"The [`pspReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_pspReference) of the payment to update. \",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character reference associated with the amount update request.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the amount update request.\
  \ Maximum length: 80 characters.\",\n      \"type\": \"string\"\n    },\n    \"splits\": {\n      \"description\": \"An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"description\": \"The status of your request. This will always have the value **received**.\",\n      \"enum\": [\n        \"received\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"merchantAccount\",\n    \"amount\",\n    \"reference\",\n    \"pspReference\",\n    \"paymentPspReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-amount-update-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentAmountUpdateResponse
---
