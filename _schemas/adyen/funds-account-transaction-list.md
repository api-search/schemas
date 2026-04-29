---
description: AccountTransactionList schema from Adyen API
layout: schema
name: AccountTransactionList
properties_list:
- description: The code of the account.
  name: accountCode
  type: string
- description: Indicates whether there is a next page of transactions available.
  name: hasNextPage
  type: boolean
- description: The list of transactions.
  name: transactions
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-account-transaction-list-schema.json
slug: funds-account-transaction-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-transaction-list-schema.json\",\n  \"title\": \"AccountTransactionList\",\n  \"description\": \"AccountTransactionList schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account.\",\n      \"type\": \"string\"\n    },\n    \"hasNextPage\": {\n      \"description\": \"Indicates whether there is a next page of transactions available.\",\n      \"type\": \"boolean\"\n    },\n    \"transactions\": {\n      \"description\": \"The list of transactions.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Transaction\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-account-transaction-list-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AccountTransactionList
---
