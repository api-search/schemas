---
description: TransactionListForAccount schema from Adyen API
layout: schema
name: TransactionListForAccount
properties_list:
- description: The account for which to retrieve the transactions.
  name: accountCode
  type: string
- description: The page of transactions to retrieve. Each page lists fifty (50) transactions. The most recent transactions are included on page 1.
  name: page
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-transaction-list-for-account-schema.json
slug: funds-transaction-list-for-account
source_filename: funds-transaction-list-for-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-transaction-list-for-account-schema.json\",\n  \"title\": \"TransactionListForAccount\",\n  \"description\": \"TransactionListForAccount schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The account for which to retrieve the transactions.\",\n      \"type\": \"string\"\n    },\n    \"page\": {\n      \"description\": \"The page of transactions to retrieve.\\nEach page lists fifty (50) transactions.  The most recent transactions are included on page 1.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"accountCode\",\n    \"page\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-transaction-list-for-account-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionListForAccount
---
