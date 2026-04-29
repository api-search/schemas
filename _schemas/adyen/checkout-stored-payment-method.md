---
description: StoredPaymentMethod schema from Adyen API
layout: schema
name: StoredPaymentMethod
properties_list:
- description: The bank account number (without separators).
  name: bankAccountNumber
  type: string
- description: The location id of the bank. The field value is `nil` in most cases.
  name: bankLocationId
  type: string
- description: The brand of the card.
  name: brand
  type: string
- description: The month the card expires.
  name: expiryMonth
  type: string
- description: The last two digits of the year the card expires. For example, **22** for the year 2022.
  name: expiryYear
  type: string
- description: The unique payment method code.
  name: holderName
  type: string
- description: The IBAN of the bank account.
  name: iban
  type: string
- description: A unique identifier of this stored payment method.
  name: id
  type: string
- description: The shopper’s issuer account label
  name: label
  type: string
- description: The last four digits of the PAN.
  name: lastFour
  type: string
- description: The display name of the stored payment method.
  name: name
  type: string
- description: Returned in the response if you are not tokenizing with Adyen and are using the Merchant-initiated transactions (MIT) framework from Mastercard or Visa. This contains either the Mastercard Trace ID or
  name: networkTxReference
  type: string
- description: The name of the bank account holder.
  name: ownerName
  type: string
- description: The shopper’s email address.
  name: shopperEmail
  type: string
- description: The supported recurring processing models for this stored payment method.
  name: supportedRecurringProcessingModels
  type: array
- description: The supported shopper interactions for this stored payment method.
  name: supportedShopperInteractions
  type: array
- description: The type of payment method.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-stored-payment-method-schema.json
slug: checkout-stored-payment-method
source_filename: checkout-stored-payment-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-stored-payment-method-schema.json\",\n  \"title\": \"StoredPaymentMethod\",\n  \"description\": \"StoredPaymentMethod schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccountNumber\": {\n      \"description\": \"The bank account number (without separators).\",\n      \"type\": \"string\"\n    },\n    \"bankLocationId\": {\n      \"description\": \"The location id of the bank. The field value is `nil` in most cases.\",\n      \"type\": \"string\"\n    },\n    \"brand\": {\n      \"description\": \"The brand of the card.\",\n      \"type\": \"string\"\n    },\n    \"expiryMonth\": {\n      \"description\": \"The month the card expires.\",\n      \"type\": \"string\"\n    },\n    \"expiryYear\": {\n      \"description\": \"The last two digits of the year the card expires. For\
  \ example, **22** for the year 2022.\",\n      \"type\": \"string\"\n    },\n    \"holderName\": {\n      \"description\": \"The unique payment method code.\",\n      \"type\": \"string\"\n    },\n    \"iban\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"The IBAN of the bank account.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"A unique identifier of this stored payment method.\",\n      \"type\": \"string\"\n    },\n    \"label\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"The shopper\\u2019s issuer account label\",\n      \"type\": \"string\"\n    },\n    \"lastFour\": {\n      \"description\": \"The last four digits of the PAN.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The display name of the stored payment method.\",\n      \"type\": \"string\"\n    },\n    \"networkTxReference\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Returned in the response\
  \ if you are not tokenizing with Adyen and are using the Merchant-initiated transactions (MIT) framework from Mastercard or Visa.\\n\\nThis contains either the Mastercard Trace ID or the Visa Transaction ID.\",\n      \"type\": \"string\"\n    },\n    \"ownerName\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"The name of the bank account holder.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper\\u2019s email address.\",\n      \"type\": \"string\"\n    },\n    \"supportedRecurringProcessingModels\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"The supported recurring processing models for this stored payment method.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"supportedShopperInteractions\": {\n      \"description\": \"The supported shopper interactions for this stored payment method.\",\n      \"items\": {\n        \"type\": \"string\"\
  \n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"The type of payment method.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-stored-payment-method-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoredPaymentMethod
---
