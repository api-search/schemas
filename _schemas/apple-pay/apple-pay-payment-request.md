---
description: Represents an ApplePayPaymentRequest used to configure an Apple Pay payment session, specifying the merchant capabilities, supported networks, payment amount, and optional shipping and billing requirements.
layout: schema
name: Apple Pay Payment Request
properties_list:
- description: The two-letter ISO 3166-1 alpha-2 country code for the merchant's country of operation
  name: countryCode
  type: string
- description: The three-letter ISO 4217 currency code for the payment
  name: currencyCode
  type: string
- description: The payment networks the merchant supports
  name: supportedNetworks
  type: array
- description: The payment capabilities the merchant supports
  name: merchantCapabilities
  type: array
- description: The total amount for the payment, including the merchant name as the label
  name: total
  type: object
- description: A list of line items explaining the charges, such as subtotal, tax, discount, and shipping
  name: lineItems
  type: array
- description: The billing contact fields required to process the payment
  name: requiredBillingContactFields
  type: array
- description: The shipping contact fields required to fulfill the order
  name: requiredShippingContactFields
  type: array
- description: Available shipping methods for the order
  name: shippingMethods
  type: array
- description: The type of shipping used for this request, which determines the wording on the payment sheet
  name: shippingType
  type: string
- description: Controls whether the shipping contact can be edited on the payment sheet
  name: shippingContactEditingMode
  type: string
- description: Base64-encoded application-specific data that is included in the payment token hash for verification
  name: applicationData
  type: string
- description: A list of ISO 3166-1 alpha-2 country codes for cards that can be used for payment. If not specified, all countries are supported
  name: supportedCountries
  type: array
- description: ''
  name: recurringPaymentRequest
  type: object
- description: ''
  name: automaticReloadPaymentRequest
  type: object
- description: An array of payment token contexts for multi-merchant payments
  name: multiTokenContexts
  type: array
provider_name: Apple Pay
provider_slug: apple-pay
schema_file: json-schema/apple-pay-payment-request-schema.json
slug: apple-pay-payment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.apple.com/schemas/apple-pay/payment-request.json\",\n  \"title\": \"Apple Pay Payment Request\",\n  \"description\": \"Represents an ApplePayPaymentRequest used to configure an Apple Pay payment session, specifying the merchant capabilities, supported networks, payment amount, and optional shipping and billing requirements.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"countryCode\",\n    \"currencyCode\",\n    \"supportedNetworks\",\n    \"merchantCapabilities\",\n    \"total\"\n  ],\n  \"properties\": {\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"The two-letter ISO 3166-1 alpha-2 country code for the merchant's country of operation\",\n      \"pattern\": \"^[A-Z]{2}$\",\n      \"examples\": [\"US\", \"GB\", \"CA\"]\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The three-letter ISO 4217 currency\
  \ code for the payment\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"examples\": [\"USD\", \"GBP\", \"EUR\"]\n    },\n    \"supportedNetworks\": {\n      \"type\": \"array\",\n      \"description\": \"The payment networks the merchant supports\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"visa\",\n          \"masterCard\",\n          \"amex\",\n          \"discover\",\n          \"jcb\",\n          \"chinaUnionPay\",\n          \"interac\",\n          \"privateLabel\",\n          \"eftpos\",\n          \"cartesBancaires\",\n          \"iD\",\n          \"quicPay\",\n          \"suica\",\n          \"mada\",\n          \"bancomat\",\n          \"bancontact\",\n          \"girocard\"\n        ]\n      },\n      \"minItems\": 1\n    },\n    \"merchantCapabilities\": {\n      \"type\": \"array\",\n      \"description\": \"The payment capabilities the merchant supports\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n  \
  \        \"supports3DS\",\n          \"supportsEMV\",\n          \"supportsCredit\",\n          \"supportsDebit\"\n        ]\n      },\n      \"minItems\": 1\n    },\n    \"total\": {\n      \"$ref\": \"#/$defs/LineItem\",\n      \"description\": \"The total amount for the payment, including the merchant name as the label\"\n    },\n    \"lineItems\": {\n      \"type\": \"array\",\n      \"description\": \"A list of line items explaining the charges, such as subtotal, tax, discount, and shipping\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LineItem\"\n      }\n    },\n    \"requiredBillingContactFields\": {\n      \"type\": \"array\",\n      \"description\": \"The billing contact fields required to process the payment\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ContactField\"\n      }\n    },\n    \"requiredShippingContactFields\": {\n      \"type\": \"array\",\n      \"description\": \"The shipping contact fields required to fulfill the order\",\n      \"items\": {\n  \
  \      \"$ref\": \"#/$defs/ContactField\"\n      }\n    },\n    \"shippingMethods\": {\n      \"type\": \"array\",\n      \"description\": \"Available shipping methods for the order\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ShippingMethod\"\n      }\n    },\n    \"shippingType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of shipping used for this request, which determines the wording on the payment sheet\",\n      \"enum\": [\n        \"shipping\",\n        \"delivery\",\n        \"storePickup\",\n        \"servicePickup\"\n      ],\n      \"default\": \"shipping\"\n    },\n    \"shippingContactEditingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Controls whether the shipping contact can be edited on the payment sheet\",\n      \"enum\": [\n        \"enabled\",\n        \"storePickup\"\n      ]\n    },\n    \"applicationData\": {\n      \"type\": \"string\",\n      \"description\": \"Base64-encoded application-specific data that is included\
  \ in the payment token hash for verification\"\n    },\n    \"supportedCountries\": {\n      \"type\": \"array\",\n      \"description\": \"A list of ISO 3166-1 alpha-2 country codes for cards that can be used for payment. If not specified, all countries are supported\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[A-Z]{2}$\"\n      }\n    },\n    \"recurringPaymentRequest\": {\n      \"$ref\": \"#/$defs/RecurringPaymentRequest\"\n    },\n    \"automaticReloadPaymentRequest\": {\n      \"$ref\": \"#/$defs/AutomaticReloadPaymentRequest\"\n    },\n    \"multiTokenContexts\": {\n      \"type\": \"array\",\n      \"description\": \"An array of payment token contexts for multi-merchant payments\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PaymentTokenContext\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"LineItem\": {\n      \"type\": \"object\",\n      \"required\": [\"label\", \"amount\"],\n      \"properties\": {\n        \"label\": {\n          \"\
  type\": \"string\",\n          \"description\": \"A short, localized description of the line item\"\n        },\n        \"amount\": {\n          \"type\": \"string\",\n          \"description\": \"The monetary amount of the line item as a string with decimal notation\",\n          \"pattern\": \"^-?\\\\d+\\\\.\\\\d{2}$\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"final\", \"pending\"],\n          \"default\": \"final\",\n          \"description\": \"Whether this is a final or pending amount\"\n        },\n        \"paymentTiming\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"immediate\",\n            \"recurring\",\n            \"deferred\",\n            \"automaticReload\"\n          ],\n          \"description\": \"When the payment will be taken\"\n        },\n        \"recurringPaymentStartDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The start\
  \ date for recurring payments\"\n        },\n        \"recurringPaymentIntervalUnit\": {\n          \"type\": \"string\",\n          \"enum\": [\"year\", \"month\", \"day\", \"hour\", \"minute\"],\n          \"description\": \"The interval unit for recurring payments\"\n        },\n        \"recurringPaymentIntervalCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The number of interval units between recurring payments\"\n        },\n        \"recurringPaymentEndDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The end date for recurring payments\"\n        },\n        \"deferredPaymentDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date for a deferred payment\"\n        },\n        \"automaticReloadPaymentThresholdAmount\": {\n          \"type\": \"string\",\n          \"description\": \"The balance threshold\
  \ that triggers an automatic reload\"\n        }\n      }\n    },\n    \"ContactField\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"email\",\n        \"name\",\n        \"phone\",\n        \"postalAddress\",\n        \"phoneticName\"\n      ],\n      \"description\": \"A contact field that can be requested from the user\"\n    },\n    \"ShippingMethod\": {\n      \"type\": \"object\",\n      \"required\": [\"label\", \"detail\", \"amount\", \"identifier\"],\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"A short description of the shipping method\"\n        },\n        \"detail\": {\n          \"type\": \"string\",\n          \"description\": \"A longer description of the shipping method\"\n        },\n        \"amount\": {\n          \"type\": \"string\",\n          \"description\": \"The cost of the shipping method\",\n          \"pattern\": \"^-?\\\\d+\\\\.\\\\d{2}$\"\n        },\n        \"identifier\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"A unique identifier for the shipping method\"\n        },\n        \"dateComponentsRange\": {\n          \"type\": \"object\",\n          \"description\": \"Estimated delivery date range\",\n          \"properties\": {\n            \"startDateComponents\": {\n              \"$ref\": \"#/$defs/DateComponents\"\n            },\n            \"endDateComponents\": {\n              \"$ref\": \"#/$defs/DateComponents\"\n            }\n          }\n        }\n      }\n    },\n    \"DateComponents\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"era\": { \"type\": \"integer\" },\n        \"year\": { \"type\": \"integer\" },\n        \"month\": { \"type\": \"integer\" },\n        \"day\": { \"type\": \"integer\" },\n        \"hours\": { \"type\": \"integer\" },\n        \"minutes\": { \"type\": \"integer\" },\n        \"seconds\": { \"type\": \"integer\" },\n        \"calendar\": { \"type\": \"string\" }\n \
  \     }\n    },\n    \"RecurringPaymentRequest\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"paymentDescription\",\n        \"regularBilling\",\n        \"managementURL\"\n      ],\n      \"description\": \"Configuration for recurring payments\",\n      \"properties\": {\n        \"paymentDescription\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the recurring payment\"\n        },\n        \"regularBilling\": {\n          \"$ref\": \"#/$defs/LineItem\",\n          \"description\": \"The regular billing amount and interval\"\n        },\n        \"trialBilling\": {\n          \"$ref\": \"#/$defs/LineItem\",\n          \"description\": \"The trial billing amount and interval, if applicable\"\n        },\n        \"billingAgreement\": {\n          \"type\": \"string\",\n          \"description\": \"A localized billing agreement for display to the user\"\n        },\n        \"managementURL\": {\n          \"type\": \"string\",\n\
  \          \"format\": \"uri\",\n          \"description\": \"A URL to manage the recurring payment\"\n        },\n        \"tokenNotificationURL\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A URL for receiving lifecycle notifications for the merchant token\"\n        }\n      }\n    },\n    \"AutomaticReloadPaymentRequest\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"paymentDescription\",\n        \"automaticReloadBilling\",\n        \"managementURL\"\n      ],\n      \"description\": \"Configuration for automatic reload payments (e.g., store cards)\",\n      \"properties\": {\n        \"paymentDescription\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the automatic reload payment\"\n        },\n        \"automaticReloadBilling\": {\n          \"$ref\": \"#/$defs/LineItem\",\n          \"description\": \"The automatic reload billing amount\"\n        },\n        \"billingAgreement\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"A localized billing agreement for display\"\n        },\n        \"managementURL\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A URL to manage the automatic reload\"\n        },\n        \"tokenNotificationURL\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A URL for receiving lifecycle notifications\"\n        }\n      }\n    },\n    \"PaymentTokenContext\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"merchantIdentifier\",\n        \"externalIdentifier\",\n        \"merchantName\",\n        \"merchantDomain\",\n        \"amount\"\n      ],\n      \"description\": \"Context for multi-merchant payment tokens\",\n      \"properties\": {\n        \"merchantIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"The merchant identifier for this context\"\n        },\n        \"\
  externalIdentifier\": {\n          \"type\": \"string\",\n          \"description\": \"An external identifier for the merchant\"\n        },\n        \"merchantName\": {\n          \"type\": \"string\",\n          \"description\": \"The merchant's display name\"\n        },\n        \"merchantDomain\": {\n          \"type\": \"string\",\n          \"description\": \"The merchant's domain\"\n        },\n        \"amount\": {\n          \"type\": \"string\",\n          \"description\": \"The amount for this merchant's portion\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/json-schema/apple-pay-payment-request-schema.json
tags:
- Apple
- Contactless Payments
- Digital Wallet
- E-Commerce
- Mobile Payments
- Payments
title: Apple Pay Payment Request
---
