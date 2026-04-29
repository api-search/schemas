---
description: JSON Schema for a Broadridge brokerage account transaction.
layout: schema
name: Broadridge Transaction
properties_list:
- description: ''
  name: transactionId
  type: string
- description: ''
  name: accountNumber
  type: string
- description: ''
  name: tradeDate
  type: string
- description: ''
  name: settleDate
  type: string
- description: ''
  name: transactionType
  type: string
- description: ''
  name: cusip
  type: string
- description: ''
  name: symbol
  type: string
- description: ''
  name: securityDescription
  type: string
- description: ''
  name: quantity
  type: number
- description: ''
  name: price
  type: number
- description: Net transaction amount after commissions and fees
  name: netAmount
  type: number
- description: Gross transaction amount before commissions and fees
  name: grossAmount
  type: number
- description: ''
  name: commission
  type: number
- description: ''
  name: fees
  type: number
- description: ''
  name: currency
  type: string
provider_name: broadridge
provider_slug: broadridge
schema_file: json-schema/broadridge-transaction-schema.json
slug: broadridge-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/json-schema/broadridge-transaction-schema.json\",\n  \"title\": \"Broadridge Transaction\",\n  \"description\": \"JSON Schema for a Broadridge brokerage account transaction.\",\n  \"type\": \"object\",\n  \"required\": [\"transactionId\", \"accountNumber\", \"transactionType\", \"tradeDate\", \"netAmount\"],\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\"\n    },\n    \"tradeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"settleDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"transactionType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Buy\", \"Sell\", \"Dividend\", \"Interest\", \"Transfer\", \"Fee\", \"Deposit\", \"Withdrawal\", \"Reinvestment\"]\n    },\n\
  \    \"cusip\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z0-9]{9}$\"\n    },\n    \"symbol\": {\n      \"type\": \"string\"\n    },\n    \"securityDescription\": {\n      \"type\": \"string\"\n    },\n    \"quantity\": {\n      \"type\": \"number\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"minimum\": 0\n    },\n    \"netAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Net transaction amount after commissions and fees\"\n    },\n    \"grossAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Gross transaction amount before commissions and fees\"\n    },\n    \"commission\": {\n      \"type\": \"number\",\n      \"minimum\": 0\n    },\n    \"fees\": {\n      \"type\": \"number\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/json-schema/broadridge-transaction-schema.json
tags: []
title: Broadridge Transaction
---
