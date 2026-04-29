---
description: TransactionRuleResponse schema from Adyen API
layout: schema
name: TransactionRuleResponse
properties_list:
- description: The transaction rule.
  name: transactionRule
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transaction-rule-response-schema.json
slug: configuration-transaction-rule-response
source_filename: configuration-transaction-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-response-schema.json\",\n  \"title\": \"TransactionRuleResponse\",\n  \"description\": \"TransactionRuleResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionRule\": {\n      \"description\": \"The transaction rule.\",\n      \"$ref\": \"#/components/schemas/TransactionRule\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transaction-rule-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRuleResponse
---
