---
description: Paginated transaction list
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
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/transactionlistresponse-schema.json
slug: transactionlistresponse
source_filename: transactionlistresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/transactionlistresponse-schema.json\",\n  \"title\": \"TransactionListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated transaction list\",\n  \"properties\": {\n    \"transactions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Transaction\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/transactionlistresponse-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: TransactionListResponse
---
