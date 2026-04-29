---
description: AdditionalDataWallets schema from Adyen API
layout: schema
name: AdditionalDataWallets
properties_list:
- description: The Android Pay token retrieved from the SDK.
  name: androidpay.token
  type: string
- description: The Mastercard Masterpass Transaction ID retrieved from the SDK.
  name: masterpass.transactionId
  type: string
- description: The Apple Pay token retrieved from the SDK.
  name: payment.token
  type: string
- description: The Google Pay token retrieved from the SDK.
  name: paywithgoogle.token
  type: string
- description: The Samsung Pay token retrieved from the SDK.
  name: samsungpay.token
  type: string
- description: The Visa Checkout Call ID retrieved from the SDK.
  name: visacheckout.callId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-additional-data-wallets-schema.json
slug: checkout-additional-data-wallets
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-wallets-schema.json\",\n  \"title\": \"AdditionalDataWallets\",\n  \"description\": \"AdditionalDataWallets schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"androidpay.token\": {\n      \"description\": \"The Android Pay token retrieved from the SDK.\",\n      \"type\": \"string\"\n    },\n    \"masterpass.transactionId\": {\n      \"description\": \"The Mastercard Masterpass Transaction ID retrieved from the SDK.\",\n      \"type\": \"string\"\n    },\n    \"payment.token\": {\n      \"description\": \"The Apple Pay token retrieved from the SDK.\",\n      \"type\": \"string\"\n    },\n    \"paywithgoogle.token\": {\n      \"description\": \"The Google Pay token retrieved from the SDK.\",\n      \"type\": \"string\"\n    },\n    \"samsungpay.token\": {\n    \
  \  \"description\": \"The Samsung Pay token retrieved from the SDK.\",\n      \"type\": \"string\"\n    },\n    \"visacheckout.callId\": {\n      \"description\": \"The Visa Checkout Call ID retrieved from the SDK.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-wallets-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataWallets
---
