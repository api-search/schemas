---
description: LoyaltyTransaction schema from Adyen API
layout: schema
name: LoyaltyTransaction
properties_list:
- description: ''
  name: LoyaltyTransactionType
  type: object
- description: ''
  name: Currency
  type: string
- description: ''
  name: TotalAmount
  type: number
- description: ''
  name: OriginalPOITransaction
  type: object
- description: ''
  name: TransactionConditions
  type: object
- description: ''
  name: SaleItem
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-transaction-schema.json
slug: terminal-loyalty-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-transaction-schema.json\",\n  \"title\": \"LoyaltyTransaction\",\n  \"description\": \"LoyaltyTransaction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoyaltyTransactionType\": {\n      \"$ref\": \"#/components/schemas/LoyaltyTransactionType\"\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\"\n    },\n    \"TotalAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"OriginalPOITransaction\": {\n      \"$ref\": \"#/components/schemas/OriginalPOITransaction\"\n    },\n    \"TransactionConditions\": {\n      \"$ref\": \"#/components/schemas/TransactionConditions\"\n    },\n    \"SaleItem\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SaleItem\"\
  \n      }\n    }\n  },\n  \"required\": [\n    \"LoyaltyTransactionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-transaction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyTransaction
---
