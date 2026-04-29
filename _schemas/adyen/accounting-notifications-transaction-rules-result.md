---
description: TransactionRulesResult schema from Adyen API
layout: schema
name: TransactionRulesResult
properties_list:
- description: The advice given by the Risk analysis.
  name: advice
  type: string
- description: Indicates whether the transaction passed the evaluation for all transaction rules.
  name: allRulesPassed
  type: boolean
- description: Array containing all the transaction rules that the transaction violated. This list is only sent when `allRulesPassed` is **false**.
  name: failedTransactionRules
  type: array
- description: The score of the Risk analysis.
  name: score
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-transaction-rules-result-schema.json
slug: accounting-notifications-transaction-rules-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transaction-rules-result-schema.json\",\n  \"title\": \"TransactionRulesResult\",\n  \"description\": \"TransactionRulesResult schema from Adyen API\",\n  \"properties\": {\n    \"advice\": {\n      \"description\": \"The advice given by the Risk analysis.\",\n      \"type\": \"string\"\n    },\n    \"allRulesPassed\": {\n      \"description\": \"Indicates whether the transaction passed the evaluation for all transaction rules.\",\n      \"type\": \"boolean\"\n    },\n    \"failedTransactionRules\": {\n      \"description\": \"Array containing all the transaction rules that the transaction violated. This list is only sent when `allRulesPassed` is **false**.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionEventViolation\"\n      },\n      \"type\": \"array\"\n\
  \    },\n    \"score\": {\n      \"description\": \"The score of the Risk analysis.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-transaction-rules-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRulesResult
---
