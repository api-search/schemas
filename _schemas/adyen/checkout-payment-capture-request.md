---
description: PaymentCaptureRequest schema from Adyen API
layout: schema
name: PaymentCaptureRequest
properties_list:
- description: The amount that you want to capture. The `currency` must match the currency used in authorisation, the `value` must be smaller than or equal to the authorised amount.
  name: amount
  type: object
- description: Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).
  name: applicationInfo
  type: object
- description: Price and product information of the refunded items, required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment). > This field is required for partial refunds with 3
  name: lineItems
  type: array
- description: The merchant account that is used to process the payment.
  name: merchantAccount
  type: string
- description: Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).
  name: platformChargebackLogic
  type: object
- description: 'Your reference for the capture request. Maximum length: 80 characters.'
  name: reference
  type: string
- description: An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-a
  name: splits
  type: array
- description: A List of sub-merchants.
  name: subMerchants
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-capture-request-schema.json
slug: checkout-payment-capture-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-capture-request-schema.json\",\n  \"title\": \"PaymentCaptureRequest\",\n  \"description\": \"PaymentCaptureRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount that you want to capture. The `currency` must match the currency used in authorisation, the `value` must be smaller than or equal to the authorised amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"applicationInfo\": {\n      \"description\": \"Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).\",\n      \"$ref\": \"#/components/schemas/ApplicationInfo\"\n    },\n    \"lineItems\": {\n      \"description\": \"Price and product information\
  \ of the refunded items, required for [partial refunds](https://docs.adyen.com/online-payments/refund#refund-a-payment).\\n> This field is required for partial refunds with 3x 4x Oney, Affirm, Afterpay, Atome, Clearpay, Klarna, Ratepay, Walley, and Zip.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that is used to process the payment.\",\n      \"type\": \"string\"\n    },\n    \"platformChargebackLogic\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).\",\n      \"$ref\": \"#/components/schemas/PlatformChargebackLogic\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the capture request. Maximum length: 80 characters.\",\n      \"type\"\
  : \"string\"\n    },\n    \"splits\": {\n      \"description\": \"An array of objects specifying how the amount should be split between accounts when using Adyen for Platforms. For details, refer to [Providing split information](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"subMerchants\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"A List of sub-merchants.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SubMerchantInfo\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-capture-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentCaptureRequest
---
