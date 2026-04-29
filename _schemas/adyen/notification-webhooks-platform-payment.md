---
description: PlatformPayment schema from Adyen API
layout: schema
name: PlatformPayment
properties_list:
- description: The account given in the related split.
  name: account
  type: string
- description: The description of the related split.
  name: description
  type: string
- description: The merchant reference of the modification.
  name: modificationMerchantReference
  type: string
- description: The pspReference of the modification.
  name: modificationPspReference
  type: string
- description: The merchant reference of the payment.
  name: paymentMerchantReference
  type: string
- description: The pspReference of the payment.
  name: paymentPspReference
  type: string
- description: The reference of the related split.
  name: reference
  type: string
- description: The type of the related split.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-platform-payment-schema.json
slug: notification-webhooks-platform-payment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-platform-payment-schema.json\",\n  \"title\": \"PlatformPayment\",\n  \"description\": \"PlatformPayment schema from Adyen API\",\n  \"properties\": {\n    \"account\": {\n      \"description\": \"The account given in the related split.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"The description of the related split.\",\n      \"type\": \"string\"\n    },\n    \"modificationMerchantReference\": {\n      \"description\": \"The merchant reference of the modification.\",\n      \"type\": \"string\"\n    },\n    \"modificationPspReference\": {\n      \"description\": \"The pspReference of the modification.\",\n      \"type\": \"string\"\n    },\n    \"paymentMerchantReference\": {\n      \"description\": \"The merchant reference of the payment.\",\n\
  \      \"type\": \"string\"\n    },\n    \"paymentPspReference\": {\n      \"description\": \"The pspReference of the payment.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The reference of the related split.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of the related split.\",\n      \"enum\": [\n        \"BalanceAccount\",\n        \"Commission\",\n        \"Default\",\n        \"PaymentFee\",\n        \"VAT\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-platform-payment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PlatformPayment
---
