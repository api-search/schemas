---
description: Paginated list of transactions
layout: schema
name: TransactionListResponse
properties_list:
- description: ''
  name: transactions
  type: array
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/transactionlistresponse-schema.json
slug: transactionlistresponse
source_filename: transactionlistresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/transactionlistresponse-schema.json\",\n  \"title\": \"TransactionListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of transactions\",\n  \"properties\": {\n    \"transactions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Transaction\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/transactionlistresponse-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: TransactionListResponse
---
