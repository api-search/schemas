---
description: PerformedTransaction schema from Adyen API
layout: schema
name: PerformedTransaction
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: SaleData
  type: object
- description: ''
  name: POIData
  type: object
- description: ''
  name: PaymentResult
  type: object
- description: ''
  name: LoyaltyResult
  type: array
- description: ''
  name: ReversedAmount
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-performed-transaction-schema.json
slug: terminal-performed-transaction
source_filename: terminal-performed-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-performed-transaction-schema.json\",\n  \"title\": \"PerformedTransaction\",\n  \"description\": \"PerformedTransaction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"SaleData\": {\n      \"$ref\": \"#/components/schemas/SaleData\"\n    },\n    \"POIData\": {\n      \"$ref\": \"#/components/schemas/POIData\"\n    },\n    \"PaymentResult\": {\n      \"$ref\": \"#/components/schemas/PaymentResult\"\n    },\n    \"LoyaltyResult\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LoyaltyResult\"\n      }\n    },\n    \"ReversedAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\n\
  \    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-performed-transaction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PerformedTransaction
---
