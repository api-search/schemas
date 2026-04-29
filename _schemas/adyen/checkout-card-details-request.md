---
description: CardDetailsRequest schema from Adyen API
layout: schema
name: CardDetailsRequest
properties_list:
- description: A minimum of the first 8 digits of the card number and a maximum of the full card number. 11 digits gives the best result. You must be [fully PCI compliant](https://docs.adyen.com/development-resource
  name: cardNumber
  type: string
- description: 'The shopper country. Format: [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) Example: NL or DE'
  name: countryCode
  type: string
- description: The encrypted card number.
  name: encryptedCardNumber
  type: string
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The card brands you support. This is the [`brands`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/paymentMethods__resParam_paymentMethods-brands) array from your [`/paymentMethods`
  name: supportedBrands
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-card-details-request-schema.json
slug: checkout-card-details-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-card-details-request-schema.json\",\n  \"title\": \"CardDetailsRequest\",\n  \"description\": \"CardDetailsRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardNumber\": {\n      \"description\": \"A minimum of the first 8 digits of the card number and a maximum of the full card number. 11 digits gives the best result. \\n\\nYou must be [fully PCI compliant](https://docs.adyen.com/development-resources/pci-dss-compliance-guide) to collect raw card data.\",\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"description\": \"The shopper country.\\n\\nFormat: [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)\\nExample: NL or DE\",\n      \"type\": \"string\"\n    },\n    \"encryptedCardNumber\": {\n      \"description\": \"The encrypted\
  \ card number.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"supportedBrands\": {\n      \"description\": \"The card brands you support. This is the [`brands`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/paymentMethods__resParam_paymentMethods-brands) array from your [`/paymentMethods`](https://docs.adyen.com/api-explorer/#/CheckoutService/latest/post/paymentMethods) response. \\n\\nIf not included, our API uses the ones configured for your merchant account and, if provided, the country code.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"cardNumber\",\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-card-details-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardDetailsRequest
---
