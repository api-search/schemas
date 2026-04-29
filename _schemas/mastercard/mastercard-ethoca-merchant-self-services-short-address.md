---
description: Address.
layout: schema
name: ShortAddress
properties_list:
- description: The street detail for the address.
  name: addressLine1
  type: string
- description: The secondary street detail for the address.
  name: addressLine2
  type: string
- description: Region where merchant's legal office is located
  name: regionCode
  type: string
- description: City where merchant's legal office is located
  name: city
  type: string
- description: The zip/postal detail for the merchant's legal address
  name: postalCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-short-address-schema.json
slug: mastercard-ethoca-merchant-self-services-short-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShortAddress\",\n  \"type\": \"object\",\n  \"description\": \"Address.\",\n  \"properties\": {\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"The street detail for the address.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"The secondary street detail for the address.\"\n    },\n    \"regionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Region where merchant's legal office is located\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where merchant's legal office is located\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The zip/postal detail for the merchant's legal address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-short-address-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: ShortAddress
---
