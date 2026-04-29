---
description: TransactionRuleReference schema from Adyen API
layout: schema
name: TransactionRuleReference
properties_list:
- description: The description of the resource.
  name: description
  type: string
- description: The unique identifier of the resource.
  name: id
  type: string
- description: The outcome type of the rule.
  name: outcomeType
  type: string
- description: The reference for the resource.
  name: reference
  type: string
- description: The score of the rule in case it's a scoreBased rule.
  name: score
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-transaction-rule-reference-schema.json
slug: transfer-webhooks-transaction-rule-reference
source_filename: transfer-webhooks-transaction-rule-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transaction-rule-reference-schema.json\",\n  \"title\": \"TransactionRuleReference\",\n  \"description\": \"TransactionRuleReference schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description of the resource.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the resource.\",\n      \"type\": \"string\"\n    },\n    \"outcomeType\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The outcome type of the rule.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The reference for the resource.\",\n      \"type\": \"string\"\n    },\n    \"score\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The score\
  \ of the rule in case it's a scoreBased rule.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transaction-rule-reference-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionRuleReference
---
