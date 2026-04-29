---
description: TransactionRulesResult schema from Adyen API
layout: schema
name: TransactionRulesResult
properties_list:
- description: The advice given by the Risk analysis.
  name: advice
  type: string
- description: Indicates whether the transaction passed the evaluation for all hardblock rules
  name: allHardBlockRulesPassed
  type: boolean
- description: The score of the Risk analysis.
  name: score
  type: integer
- description: Array containing all the transaction rules that the transaction triggered.
  name: triggeredTransactionRules
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-transaction-rules-result-schema.json
slug: transfer-webhooks-transaction-rules-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transaction-rules-result-schema.json\",\n  \"title\": \"TransactionRulesResult\",\n  \"description\": \"TransactionRulesResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"advice\": {\n      \"description\": \"The advice given by the Risk analysis.\",\n      \"type\": \"string\"\n    },\n    \"allHardBlockRulesPassed\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"Indicates whether the transaction passed the evaluation for all hardblock rules\",\n      \"type\": \"boolean\"\n    },\n    \"score\": {\n      \"description\": \"The score of the Risk analysis.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"triggeredTransactionRules\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"Array containing all\
  \ the transaction rules that the transaction triggered.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionEventViolation\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transaction-rules-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRulesResult
---
