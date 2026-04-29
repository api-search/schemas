---
description: Conditions on which the transaction must be processed.
layout: schema
name: TransactionConditions
properties_list:
- description: ''
  name: AllowedPaymentBrand
  type: array
- description: ''
  name: AcquirerID
  type: array
- description: The preferred type of payment is a debit transaction rather a credit transaction.
  name: DebitPreferredFlag
  type: boolean
- description: ''
  name: AllowedLoyaltyBrand
  type: array
- description: ''
  name: LoyaltyHandling
  type: object
- description: If the language is selected by the Sale System before the request to the POI.
  name: CustomerLanguage
  type: string
- description: Go online if data sent.
  name: ForceOnlineFlag
  type: boolean
- description: ''
  name: ForceEntryMode
  type: object
- description: The payment implies a specific MCC.
  name: MerchantCategoryCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-transaction-conditions-schema.json
slug: terminal-transaction-conditions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-conditions-schema.json\",\n  \"title\": \"TransactionConditions\",\n  \"description\": \"Conditions on which the transaction must be processed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowedPaymentBrand\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^.+$\",\n        \"description\": \"Restrict brand if data sent.\"\n      }\n    },\n    \"AcquirerID\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"description\": \"Restrict to these Acquirer if present.\"\n      }\n    },\n    \"DebitPreferredFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"The preferred type of payment is a debit transaction rather a credit transaction.\"\n    },\n    \"AllowedLoyaltyBrand\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^.+$\",\n        \"description\": \"Restrict brand if data sent.\"\n      }\n    },\n    \"LoyaltyHandling\": {\n      \"$ref\": \"#/components/schemas/LoyaltyHandling\"\n    },\n    \"CustomerLanguage\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\",\n      \"description\": \"If the language is selected by the Sale System before the request to the POI.\"\n    },\n    \"ForceOnlineFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Go online if data sent.\"\n    },\n    \"ForceEntryMode\": {\n      \"$ref\": \"#/components/schemas/ForceEntryMode\"\n    },\n    \"MerchantCategoryCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.{3,4}$\",\n      \"description\": \"The payment implies a specific MCC.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-conditions-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionConditions
---
