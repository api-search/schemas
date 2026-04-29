---
description: PaymentTransaction schema from Adyen API
layout: schema
name: PaymentTransaction
properties_list:
- description: ''
  name: AmountsReq
  type: object
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
schema_file: json-schema/terminal-payment-transaction-schema.json
slug: terminal-payment-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-transaction-schema.json\",\n  \"title\": \"PaymentTransaction\",\n  \"description\": \"PaymentTransaction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AmountsReq\": {\n      \"$ref\": \"#/components/schemas/AmountsReq\"\n    },\n    \"OriginalPOITransaction\": {\n      \"$ref\": \"#/components/schemas/OriginalPOITransaction\"\n    },\n    \"TransactionConditions\": {\n      \"$ref\": \"#/components/schemas/TransactionConditions\"\n    },\n    \"SaleItem\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SaleItem\"\n      }\n    }\n  },\n  \"required\": [\n    \"AmountsReq\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-transaction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentTransaction
---
