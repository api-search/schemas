---
description: TransactionRulesResponse schema from Adyen API
layout: schema
name: TransactionRulesResponse
properties_list:
- description: List of transaction rules.
  name: transactionRules
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transaction-rules-response-schema.json
slug: configuration-transaction-rules-response
source_filename: configuration-transaction-rules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rules-response-schema.json\",\n  \"title\": \"TransactionRulesResponse\",\n  \"description\": \"TransactionRulesResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionRules\": {\n      \"description\": \"List of transaction rules.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransactionRule\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rules-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRulesResponse
---
