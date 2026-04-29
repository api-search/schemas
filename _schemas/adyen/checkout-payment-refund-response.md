---
description: PaymentRefundResponse schema from Adyen API
layout: schema
name: PaymentRefundResponse
properties_list:
- description: The refund amount.
  name: amount
  type: object
- description: Price and product information of the refunded items, required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment). > This field is required for partial refunds with 3
  name: lineItems
  type: array
- description: The merchant account that is used to process the payment.
  name: merchantAccount
  type: string
- description: Your reason for the refund request.
  name: merchantRefundReason
  type: string
- description: The [`pspReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_pspReference) of the payment to refund.
  name: paymentPspReference
  type: string
- description: Adyen's 16-character reference associated with the refund request.
  name: pspReference
  type: string
- description: Your reference for the refund request.
  name: reference
  type: string
- description: An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-a
  name: splits
  type: array
- description: The status of your request. This will always have the value **received**.
  name: status
  type: string
- description: The online store or [physical store](https://docs.adyen.com/point-of-sale/design-your-integration/determine-account-structure/#create-stores) that is processing the refund. This must be the same as th
  name: store
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-refund-response-schema.json
slug: checkout-payment-refund-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-refund-response-schema.json\",\n  \"title\": \"PaymentRefundResponse\",\n  \"description\": \"PaymentRefundResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The refund amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"lineItems\": {\n      \"description\": \"Price and product information of the refunded items, required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment).\\n> This field is required for partial refunds with 3x 4x Oney, Affirm, Afterpay, Atome, Clearpay, Klarna, Ratepay, Walley, and Zip.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccount\": {\n      \"description\"\
  : \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"merchantRefundReason\": {\n      \"description\": \"Your reason for the refund request.\",\n      \"enum\": [\n        \"FRAUD\",\n        \"CUSTOMER REQUEST\",\n        \"RETURN\",\n        \"DUPLICATE\",\n        \"OTHER\"\n      ],\n      \"type\": \"string\"\n    },\n    \"paymentPspReference\": {\n      \"description\": \"The [`pspReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_pspReference) of the payment to refund. \",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character reference associated with the refund request.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the refund request.\",\n      \"type\": \"string\"\n    },\n    \"splits\": {\n      \"description\": \"An array of objects specifying how the amount should\
  \ be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"description\": \"The status of your request. This will always have the value **received**.\",\n      \"enum\": [\n        \"received\"\n      ],\n      \"type\": \"string\"\n    },\n    \"store\": {\n      \"description\": \"The online store or [physical store](https://docs.adyen.com/point-of-sale/design-your-integration/determine-account-structure/#create-stores) that is processing the refund. This must be the same as the store name configured in your Customer Area.  Otherwise, you get an error and the refund fails.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"merchantAccount\",\n    \"amount\"\
  ,\n    \"pspReference\",\n    \"paymentPspReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-refund-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentRefundResponse
---
