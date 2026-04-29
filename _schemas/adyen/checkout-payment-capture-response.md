---
description: PaymentCaptureResponse schema from Adyen API
layout: schema
name: PaymentCaptureResponse
properties_list:
- description: The captured amount.
  name: amount
  type: object
- description: Price and product information of the refunded items, required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment). > This field is required for partial refunds with 3
  name: lineItems
  type: array
- description: The merchant account that is used to process the payment.
  name: merchantAccount
  type: string
- description: The [`pspReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_pspReference) of the payment to capture.
  name: paymentPspReference
  type: string
- description: Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).
  name: platformChargebackLogic
  type: object
- description: Adyen's 16-character reference associated with the capture request.
  name: pspReference
  type: string
- description: Your reference for the capture request.
  name: reference
  type: string
- description: An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-a
  name: splits
  type: array
- description: The status of your request. This will always have the value **received**.
  name: status
  type: string
- description: List of sub-merchants.
  name: subMerchants
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-capture-response-schema.json
slug: checkout-payment-capture-response
source_filename: checkout-payment-capture-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-capture-response-schema.json\",\n  \"title\": \"PaymentCaptureResponse\",\n  \"description\": \"PaymentCaptureResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The captured amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"lineItems\": {\n      \"description\": \"Price and product information of the refunded items, required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment).\\n> This field is required for partial refunds with 3x 4x Oney, Affirm, Afterpay, Atome, Clearpay, Klarna, Ratepay, Walley, and Zip.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccount\": {\n      \"description\"\
  : \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"paymentPspReference\": {\n      \"description\": \"The [`pspReference`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/payments__resParam_pspReference) of the payment to capture. \",\n      \"type\": \"string\"\n    },\n    \"platformChargebackLogic\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).\",\n      \"$ref\": \"#/components/schemas/PlatformChargebackLogic\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character reference associated with the capture request.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the capture request.\",\n      \"type\": \"string\"\n    },\n    \"splits\": {\n      \"description\"\
  : \"An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"description\": \"The status of your request. This will always have the value **received**.\",\n      \"enum\": [\n        \"received\"\n      ],\n      \"type\": \"string\"\n    },\n    \"subMerchants\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"List of sub-merchants.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubMerchantInfo\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"merchantAccount\",\n    \"amount\",\n    \"pspReference\",\n    \"paymentPspReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-capture-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentCaptureResponse
---
