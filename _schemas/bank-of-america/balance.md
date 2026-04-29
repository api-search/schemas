---
description: Account balance information
layout: schema
name: Balance
properties_list:
- description: Account identifier
  name: accountId
  type: string
- description: Current ledger balance
  name: ledgerBalance
  type: number
- description: Available balance for transactions
  name: availableBalance
  type: number
- description: Collected balance after float
  name: collectedBalance
  type: number
- description: Balance currency (ISO 4217)
  name: currency
  type: string
- description: Balance as of timestamp
  name: asOfDate
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/balance-schema.json
slug: balance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/balance-schema.json\",\n  \"title\": \"Balance\",\n  \"type\": \"object\",\n  \"description\": \"Account balance information\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account identifier\"\n    },\n    \"ledgerBalance\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Current ledger balance\"\n    },\n    \"availableBalance\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Available balance for transactions\"\n    },\n    \"collectedBalance\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Collected balance after float\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Balance currency (ISO 4217)\"\n    },\n    \"asOfDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Balance as of timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/balance-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Balance
---
