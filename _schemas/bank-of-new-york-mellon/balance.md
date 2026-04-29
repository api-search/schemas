---
description: Account balance record
layout: schema
name: Balance
properties_list:
- description: ''
  name: accountId
  type: string
- description: Balance type (current, available, intraday)
  name: balanceType
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: asOfDateTime
  type: string
- description: ''
  name: openingBalance
  type: number
- description: ''
  name: closingBalance
  type: number
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
schema_file: json-schema/balance-schema.json
slug: balance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-new-york-mellon/json-schema/balance-schema.json\",\n  \"title\": \"Balance\",\n  \"type\": \"object\",\n  \"description\": \"Account balance record\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"balanceType\": {\n      \"type\": \"string\",\n      \"description\": \"Balance type (current, available, intraday)\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"asOfDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"openingBalance\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"closingBalance\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/json-schema/balance-schema.json
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
title: Balance
---
