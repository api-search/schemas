---
description: AdjustTransactionModel schema from Avalara API
layout: schema
name: AdjustTransactionModel
properties_list:
- description: ''
  name: adjustmentReason
  type: string
- description: ''
  name: adjustmentDescription
  type: string
- description: ''
  name: newTransaction
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-adjust-transaction-model-schema.json
slug: avatax-rest-adjust-transaction-model
source_filename: avatax-rest-adjust-transaction-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-adjust-transaction-model-schema.json\",\n  \"title\": \"AdjustTransactionModel\",\n  \"description\": \"AdjustTransactionModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"adjustmentReason\",\n    \"newTransaction\"\n  ],\n  \"properties\": {\n    \"adjustmentReason\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NotAdjusted\",\n        \"SourcingIssue\",\n        \"ReconciledWithGeneralLedger\",\n        \"ExemptCertApplied\",\n        \"PriceAdjusted\",\n        \"ProductReturned\",\n        \"ProductExchanged\",\n        \"BadDebt\",\n        \"Other\"\n      ]\n    },\n    \"adjustmentDescription\": {\n      \"type\": \"string\"\n    },\n    \"newTransaction\": {\n      \"$ref\": \"#/components/schemas/CreateTransactionModel\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-adjust-transaction-model-schema.json
tags:
- Taxes
title: AdjustTransactionModel
---
