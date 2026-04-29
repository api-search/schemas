---
description: PaymentMethodsRequest schema from Adyen API
layout: schema
name: PaymentMethodsRequest
properties_list:
- description: This field contains additional data, which may be required for a particular payment request. The `additionalData` object consists of entries, each of which includes the key and value.
  name: additionalData
  type: object
- description: 'List of payment methods to be presented to the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types). Example: `"allowedPay'
  name: allowedPaymentMethods
  type: array
- description: The amount information for the transaction (in [minor units](https://docs.adyen.com/development-resources/currency-codes)). For [BIN or card verification](https://docs.adyen.com/payment-methods/cards/
  name: amount
  type: object
- description: 'List of payment methods to be hidden from the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types). Example: `"blockedPaym'
  name: blockedPaymentMethods
  type: array
- description: 'The platform where a payment transaction takes place. This field can be used for filtering out payment methods that are only available on specific platforms. Possible values: * iOS * Android * Web'
  name: channel
  type: string
- description: The shopper's country code.
  name: countryCode
  type: string
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The order information required for partial payments.
  name: order
  type: object
- description: The combination of a language code and a country code to specify the language to be used in the payment.
  name: shopperLocale
  type: string
- description: 'Required for recurring payments. Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identif'
  name: shopperReference
  type: string
- description: Boolean value indicating whether the card payment method should be split into separate debit and credit options.
  name: splitCardFundingSources
  type: boolean
- description: Required for Adyen for Platforms integrations if you have a platform setup. This is your [reference](https://docs.adyen.com/api-explorer/Management/3/post/merchants/(merchantId)/stores#request-referen
  name: store
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-methods-request-schema.json
slug: checkout-payment-methods-request
source_filename: checkout-payment-methods-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-methods-request-schema.json\",\n  \"title\": \"PaymentMethodsRequest\",\n  \"description\": \"PaymentMethodsRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalData3DSecure\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataAirline\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataCarRental\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataCommon\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataLevel23\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataLodging\"\
  \n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataOpenInvoice\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataOpi\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRatepay\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRetry\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRisk\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRiskStandalone\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataSubMerchant\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataTemporaryServices\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataWallets\"\n        }\n      ],\n      \"description\": \"This field contains additional data, which may be required for a particular payment request.\\n\\nThe `additionalData`\
  \ object consists of entries, each of which includes the key and value.\",\n      \"type\": \"object\"\n    },\n    \"allowedPaymentMethods\": {\n      \"x-addedInVersion\": \"33\",\n      \"description\": \"List of payment methods to be presented to the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types).\\n\\nExample: `\\\"allowedPaymentMethods\\\":[\\\"ideal\\\",\\\"giropay\\\"]`\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"amount\": {\n      \"description\": \"The amount information for the transaction (in [minor units](https://docs.adyen.com/development-resources/currency-codes)). For [BIN or card verification](https://docs.adyen.com/payment-methods/cards/bin-data-and-card-verification) requests, set amount to 0 (zero).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"blockedPaymentMethods\": {\n      \"x-addedInVersion\": \"\
  33\",\n      \"description\": \"List of payment methods to be hidden from the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types).\\n\\nExample: `\\\"blockedPaymentMethods\\\":[\\\"ideal\\\",\\\"giropay\\\"]`\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"channel\": {\n      \"description\": \"The platform where a payment transaction takes place. This field can be used for filtering out payment methods that are only available on specific platforms. Possible values:\\n* iOS\\n* Android\\n* Web\",\n      \"enum\": [\n        \"iOS\",\n        \"Android\",\n        \"Web\"\n      ],\n      \"type\": \"string\"\n    },\n    \"countryCode\": {\n      \"description\": \"The shopper's country code.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"order\": {\n      \"x-addedInVersion\": \"64\",\n      \"description\": \"The order information required for partial payments.\",\n      \"$ref\": \"#/components/schemas/EncryptedOrderData\"\n    },\n    \"shopperLocale\": {\n      \"x-addedInVersion\": \"7\",\n      \"description\": \"The combination of a language code and a country code to specify the language to be used in the payment.\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Required for recurring payments. \\nYour reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"type\": \"string\"\n    },\n    \"splitCardFundingSources\": {\n      \"x-addedInVersion\": \"53\",\n      \"default\": false,\n      \"description\": \"Boolean value indicating whether the card\
  \ payment method should be split into separate debit and credit options.\",\n      \"type\": \"boolean\"\n    },\n    \"store\": {\n      \"x-addedInVersion\": \"23\",\n      \"description\": \"Required for Adyen for Platforms integrations if you have a platform setup. This is your [reference](https://docs.adyen.com/api-explorer/Management/3/post/merchants/(merchantId)/stores#request-reference) (on [balance platform](https://docs.adyen.com/marketplaces-and-platforms/classic/platforms-for-partners#route-payments)) or the [storeReference](https://docs.adyen.com/api-explorer/Account/latest/post/updateAccountHolder#request-accountHolderDetails-storeDetails-storeReference) (in the [classic integration](https://docs.adyen.com/marketplaces-and-platforms/processing-payments/route-payment-to-store/#route-a-payment-to-a-store)) for the ecommerce or point-of-sale store that is processing the payment.\",\n      \"maxLength\": 16,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    }\n  },\n\
  \  \"required\": [\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-methods-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentMethodsRequest
---
