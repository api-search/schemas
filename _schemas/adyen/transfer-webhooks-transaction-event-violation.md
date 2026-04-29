---
description: TransactionEventViolation schema from Adyen API
layout: schema
name: TransactionEventViolation
properties_list:
- description: An explanation about why the transaction rule failed.
  name: reason
  type: string
- description: Contains information about the transaction rule.
  name: transactionRule
  type: object
- description: Contains the type and ID of the resource to which the transaction rule is linked.
  name: transactionRuleSource
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-transaction-event-violation-schema.json
slug: transfer-webhooks-transaction-event-violation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transaction-event-violation-schema.json\",\n  \"title\": \"TransactionEventViolation\",\n  \"description\": \"TransactionEventViolation schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reason\": {\n      \"description\": \"An explanation about why the transaction rule failed.\",\n      \"type\": \"string\"\n    },\n    \"transactionRule\": {\n      \"description\": \"Contains information about the transaction rule.\",\n      \"$ref\": \"#/components/schemas/TransactionRuleReference\"\n    },\n    \"transactionRuleSource\": {\n      \"description\": \"Contains the type and ID of the resource to which the transaction rule is linked.\",\n      \"$ref\": \"#/components/schemas/TransactionRuleSource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transaction-event-violation-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionEventViolation
---
