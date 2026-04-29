---
description: Account balances response
layout: schema
name: BalanceResponse
properties_list:
- description: ''
  name: accountId
  type: string
- description: ''
  name: balances
  type: array
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/balanceresponse-schema.json
slug: balanceresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/balanceresponse-schema.json\",\n  \"title\": \"BalanceResponse\",\n  \"type\": \"object\",\n  \"description\": \"Account balances response\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"balances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Balance\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/balanceresponse-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: BalanceResponse
---
