---
description: MerchantAcquirerPair schema from Adyen API
layout: schema
name: MerchantAcquirerPair
properties_list:
- description: The acquirer ID.
  name: acquirerId
  type: string
- description: The merchant identification number (MID).
  name: merchantId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-merchant-acquirer-pair-schema.json
slug: configuration-merchant-acquirer-pair
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-merchant-acquirer-pair-schema.json\",\n  \"title\": \"MerchantAcquirerPair\",\n  \"description\": \"MerchantAcquirerPair schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acquirerId\": {\n      \"description\": \"The acquirer ID.\",\n      \"type\": \"string\"\n    },\n    \"merchantId\": {\n      \"description\": \"The merchant identification number (MID).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-merchant-acquirer-pair-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MerchantAcquirerPair
---
