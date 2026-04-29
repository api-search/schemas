---
description: TransferNotificationMerchantData schema from Adyen API
layout: schema
name: TransferNotificationMerchantData
properties_list:
- description: The unique identifier of the merchant's acquirer.
  name: acquirerId
  type: string
- description: The city where the merchant is located.
  name: city
  type: string
- description: The country where the merchant is located.
  name: country
  type: string
- description: The merchant category code.
  name: mcc
  type: string
- description: The merchant identifier.
  name: merchantId
  type: string
- description: The name of the merchant's shop or service.
  name: name
  type: string
- description: The merchant postal code.
  name: postalCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-transfer-notification-merchant-data-schema.json
slug: transfer-webhooks-transfer-notification-merchant-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transfer-notification-merchant-data-schema.json\",\n  \"title\": \"TransferNotificationMerchantData\",\n  \"description\": \"TransferNotificationMerchantData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acquirerId\": {\n      \"description\": \"The unique identifier of the merchant's acquirer.\",\n      \"type\": \"string\"\n    },\n    \"city\": {\n      \"description\": \"The city where the merchant is located.\",\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The country where the merchant is located.\",\n      \"type\": \"string\"\n    },\n    \"mcc\": {\n      \"description\": \"The merchant category code.\",\n      \"type\": \"string\"\n    },\n    \"merchantId\": {\n      \"description\": \"The merchant identifier.\",\n\
  \      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the merchant's shop or service.\",\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"description\": \"The merchant postal code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transfer-notification-merchant-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferNotificationMerchantData
---
