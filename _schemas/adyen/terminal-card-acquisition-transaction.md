---
description: CardAcquisitionTransaction schema from Adyen API
layout: schema
name: CardAcquisitionTransaction
properties_list:
- description: ''
  name: AllowedPaymentBrand
  type: array
- description: ''
  name: AllowedLoyaltyBrand
  type: array
- description: ''
  name: LoyaltyHandling
  type: object
- description: ''
  name: CustomerLanguage
  type: string
- description: ''
  name: ForceEntryMode
  type: object
- description: ''
  name: ForceCustomerSelectionFlag
  type: boolean
- description: ''
  name: TotalAmount
  type: number
- description: ''
  name: PaymentType
  type: object
- description: ''
  name: CashBackFlag
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-card-acquisition-transaction-schema.json
slug: terminal-card-acquisition-transaction
source_filename: terminal-card-acquisition-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-acquisition-transaction-schema.json\",\n  \"title\": \"CardAcquisitionTransaction\",\n  \"description\": \"CardAcquisitionTransaction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowedPaymentBrand\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^.+$\"\n      }\n    },\n    \"AllowedLoyaltyBrand\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^.+$\"\n      }\n    },\n    \"LoyaltyHandling\": {\n      \"$ref\": \"#/components/schemas/LoyaltyHandling\"\n    },\n    \"CustomerLanguage\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\"\n    },\n    \"ForceEntryMode\": {\n      \"$ref\": \"#/components/schemas/ForceEntryMode\"\n   \
  \ },\n    \"ForceCustomerSelectionFlag\": {\n      \"type\": \"boolean\"\n    },\n    \"TotalAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"PaymentType\": {\n      \"$ref\": \"#/components/schemas/PaymentType\"\n    },\n    \"CashBackFlag\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-acquisition-transaction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardAcquisitionTransaction
---
