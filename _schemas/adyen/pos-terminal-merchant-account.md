---
description: MerchantAccount schema from Adyen API
layout: schema
name: MerchantAccount
properties_list:
- description: List of terminals assigned to this merchant account as in-store terminals. This means that the terminal is ready to be boarded, or is already boarded.
  name: inStoreTerminals
  type: array
- description: List of terminals assigned to the inventory of this merchant account.
  name: inventoryTerminals
  type: array
- description: The merchant account.
  name: merchantAccount
  type: string
- description: Array of stores under this merchant account.
  name: stores
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/pos-terminal-merchant-account-schema.json
slug: pos-terminal-merchant-account
source_filename: pos-terminal-merchant-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-merchant-account-schema.json\",\n  \"title\": \"MerchantAccount\",\n  \"description\": \"MerchantAccount schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inStoreTerminals\": {\n      \"description\": \"List of terminals assigned to this merchant account as in-store terminals. This means that the terminal is ready to be boarded, or is already boarded.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"inventoryTerminals\": {\n      \"description\": \"List of terminals assigned to the inventory of this merchant account.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account.\",\n      \"type\": \"string\"\
  \n    },\n    \"stores\": {\n      \"description\": \"Array of stores under this merchant account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Store\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/pos-terminal-merchant-account-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MerchantAccount
---
