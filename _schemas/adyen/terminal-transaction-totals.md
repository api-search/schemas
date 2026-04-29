---
description: If Result is Success, contains all the totals, classified as required by the Sale in the message request. At least, transaction totals are provided per Acquirer, Acquirer Settlement, and Card Brand. Result of the Sale to POI Reconciliation processing.
layout: schema
name: TransactionTotals
properties_list:
- description: ''
  name: PaymentInstrumentType
  type: object
- description: If available.
  name: AcquirerID
  type: integer
- description: If available.
  name: HostReconciliationID
  type: string
- description: If configured to present totals per card brand, and Response.Result is Success.
  name: CardBrand
  type: string
- description: If requested in the message request.
  name: POIID
  type: string
- description: If requested in the message request.
  name: SaleID
  type: string
- description: If requested in the message request.
  name: OperatorID
  type: string
- description: If requested in the message request.
  name: ShiftNumber
  type: string
- description: If requested in the message request.
  name: TotalsGroupID
  type: string
- description: Currency of a monetary amount.
  name: PaymentCurrency
  type: string
- description: ''
  name: PaymentTotals
  type: array
- description: ''
  name: LoyaltyUnit
  type: object
- description: If LoyaltyUnit is Monetary.
  name: LoyaltyCurrency
  type: string
- description: ''
  name: LoyaltyTotals
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-transaction-totals-schema.json
slug: terminal-transaction-totals
source_filename: terminal-transaction-totals-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-totals-schema.json\",\n  \"title\": \"TransactionTotals\",\n  \"description\": \"If Result is Success, contains all the totals, classified as required by the Sale in the message request. At least, transaction totals are provided per Acquirer, Acquirer Settlement, and Card Brand. Result of the Sale to POI Reconciliation processing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PaymentInstrumentType\": {\n      \"$ref\": \"#/components/schemas/PaymentInstrumentType\"\n    },\n    \"AcquirerID\": {\n      \"type\": \"integer\",\n      \"description\": \"If available.\"\n    },\n    \"HostReconciliationID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If available.\"\n    },\n    \"CardBrand\": {\n      \"type\": \"string\",\n      \"pattern\"\
  : \"^.+$\",\n      \"description\": \"If configured to present totals per card brand, and Response.Result is Success.\"\n    },\n    \"POIID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If requested in the message request.\"\n    },\n    \"SaleID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If requested in the message request.\"\n    },\n    \"OperatorID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If requested in the message request.\"\n    },\n    \"ShiftNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If requested in the message request.\"\n    },\n    \"TotalsGroupID\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{1,16}$\",\n      \"description\": \"If requested in the message request.\"\n    },\n    \"PaymentCurrency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\",\n\
  \      \"description\": \"Currency of a monetary amount.\"\n    },\n    \"PaymentTotals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentTotals\"\n      }\n    },\n    \"LoyaltyUnit\": {\n      \"$ref\": \"#/components/schemas/LoyaltyUnit\"\n    },\n    \"LoyaltyCurrency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\",\n      \"description\": \"If LoyaltyUnit is Monetary.\"\n    },\n    \"LoyaltyTotals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LoyaltyTotals\"\n      }\n    }\n  },\n  \"required\": [\n    \"PaymentInstrumentType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-totals-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionTotals
---
