---
description: SubMerchantInfo schema from Adyen API
layout: schema
name: SubMerchantInfo
properties_list:
- description: ''
  name: address
  type: object
- description: ''
  name: id
  type: string
- description: ''
  name: mcc
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: taxId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-sub-merchant-info-schema.json
slug: checkout-sub-merchant-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-sub-merchant-info-schema.json\",\n  \"title\": \"SubMerchantInfo\",\n  \"description\": \"SubMerchantInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"$ref\": \"#/components/schemas/BillingAddress\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"mcc\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"taxId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-sub-merchant-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SubMerchantInfo
---
