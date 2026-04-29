---
description: Paginated list of transactions
layout: schema
name: TransactionList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: Avaloq
provider_slug: avaloq
schema_file: json-schema/banking-transaction-list-schema.json
slug: banking-transaction-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-transaction-list-schema.json\",\n  \"title\": \"TransactionList\",\n  \"description\": \"Paginated list of transactions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Transaction\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 124\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/json-schema/banking-transaction-list-schema.json
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
title: TransactionList
---
