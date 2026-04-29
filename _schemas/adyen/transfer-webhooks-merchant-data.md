---
description: MerchantData schema from Adyen API
layout: schema
name: MerchantData
properties_list:
- description: The unique identifier of the merchant's acquirer.
  name: acquirerId
  type: string
- description: The merchant category code.
  name: mcc
  type: string
- description: The merchant identifier.
  name: merchantId
  type: string
- description: Contains the merchant's name and location.
  name: nameLocation
  type: object
- description: The merchant postal code.
  name: postalCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-merchant-data-schema.json
slug: transfer-webhooks-merchant-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-merchant-data-schema.json\",\n  \"title\": \"MerchantData\",\n  \"description\": \"MerchantData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acquirerId\": {\n      \"description\": \"The unique identifier of the merchant's acquirer.\",\n      \"type\": \"string\"\n    },\n    \"mcc\": {\n      \"description\": \"The merchant category code.\",\n      \"type\": \"string\"\n    },\n    \"merchantId\": {\n      \"description\": \"The merchant identifier.\",\n      \"type\": \"string\"\n    },\n    \"nameLocation\": {\n      \"description\": \"Contains the merchant's name and location.\",\n      \"$ref\": \"#/components/schemas/NameLocation\"\n    },\n    \"postalCode\": {\n      \"description\": \"The merchant postal code.\",\n      \"type\": \"string\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-merchant-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MerchantData
---
