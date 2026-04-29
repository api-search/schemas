---
description: CheckoutVoucherAction schema from Adyen API
layout: schema
name: CheckoutVoucherAction
properties_list:
- description: The voucher alternative reference code.
  name: alternativeReference
  type: string
- description: A collection institution number (store number) for Econtext Pay-Easy ATM.
  name: collectionInstitutionNumber
  type: string
- description: The URL to download the voucher.
  name: downloadUrl
  type: string
- description: An entity number of Multibanco.
  name: entity
  type: string
- description: The date time of the voucher expiry.
  name: expiresAt
  type: string
- description: The initial amount.
  name: initialAmount
  type: object
- description: The URL to the detailed instructions to make payment using the voucher.
  name: instructionsUrl
  type: string
- description: The issuer of the voucher.
  name: issuer
  type: string
- description: The shopper telephone number (partially masked).
  name: maskedTelephoneNumber
  type: string
- description: The merchant name.
  name: merchantName
  type: string
- description: The merchant reference.
  name: merchantReference
  type: string
- description: A base64 encoded signature of all properties
  name: passCreationToken
  type: string
- description: Encoded payment data.
  name: paymentData
  type: string
- description: Specifies the payment method.
  name: paymentMethodType
  type: string
- description: The voucher reference code.
  name: reference
  type: string
- description: The shopper email.
  name: shopperEmail
  type: string
- description: The shopper name.
  name: shopperName
  type: string
- description: The surcharge amount.
  name: surcharge
  type: object
- description: The total amount (initial plus surcharge amount).
  name: totalAmount
  type: object
- description: '**voucher**'
  name: type
  type: string
- description: Specifies the URL to redirect to.
  name: url
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-checkout-voucher-action-schema.json
slug: checkout-checkout-voucher-action
source_filename: checkout-checkout-voucher-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-voucher-action-schema.json\",\n  \"title\": \"CheckoutVoucherAction\",\n  \"description\": \"CheckoutVoucherAction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alternativeReference\": {\n      \"description\": \"The voucher alternative reference code.\",\n      \"type\": \"string\"\n    },\n    \"collectionInstitutionNumber\": {\n      \"description\": \"A collection institution number (store number) for Econtext Pay-Easy ATM.\",\n      \"type\": \"string\"\n    },\n    \"downloadUrl\": {\n      \"description\": \"The URL to download the voucher.\",\n      \"type\": \"string\"\n    },\n    \"entity\": {\n      \"description\": \"An entity number of Multibanco.\",\n      \"type\": \"string\"\n    },\n    \"expiresAt\": {\n      \"description\": \"The date time of\
  \ the voucher expiry.\",\n      \"type\": \"string\"\n    },\n    \"initialAmount\": {\n      \"description\": \"The initial amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"instructionsUrl\": {\n      \"description\": \"The URL to the detailed instructions to make payment using the voucher.\",\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"description\": \"The issuer of the voucher.\",\n      \"type\": \"string\"\n    },\n    \"maskedTelephoneNumber\": {\n      \"description\": \"The shopper telephone number (partially masked).\",\n      \"type\": \"string\"\n    },\n    \"merchantName\": {\n      \"description\": \"The merchant name.\",\n      \"type\": \"string\"\n    },\n    \"merchantReference\": {\n      \"description\": \"The merchant reference.\",\n      \"type\": \"string\"\n    },\n    \"passCreationToken\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"A base64 encoded signature of all properties\",\n      \"type\"\
  : \"string\"\n    },\n    \"paymentData\": {\n      \"description\": \"Encoded payment data.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethodType\": {\n      \"description\": \"Specifies the payment method.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The voucher reference code.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper email.\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"description\": \"The shopper name.\",\n      \"type\": \"string\"\n    },\n    \"surcharge\": {\n      \"description\": \"The surcharge amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"totalAmount\": {\n      \"description\": \"The total amount (initial plus surcharge amount).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"type\": {\n      \"description\": \"**voucher**\",\n      \"enum\": [\n        \"voucher\"\n      ],\n      \"type\"\
  : \"string\"\n    },\n    \"url\": {\n      \"description\": \"Specifies the URL to redirect to.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-voucher-action-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CheckoutVoucherAction
---
