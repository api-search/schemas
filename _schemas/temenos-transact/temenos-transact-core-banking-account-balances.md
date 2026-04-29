---
description: Balance breakdown for a banking account
layout: schema
name: AccountBalances
properties_list:
- description: Account identifier
  name: accountId
  type: string
- description: Currency of the balances
  name: currency
  type: string
- description: Current working balance including pending transactions
  name: workingBalance
  type: number
- description: Balance available for withdrawals and payments
  name: availableBalance
  type: number
- description: Balance of cleared funds only
  name: clearedBalance
  type: number
- description: Amount locked or blocked on the account
  name: lockedAmount
  type: number
- description: Approved overdraft facility amount
  name: overdraftLimit
  type: number
- description: Interest accrued but not yet capitalized
  name: accruedInterest
  type: number
- description: Deposits received but not yet cleared
  name: pendingDeposits
  type: number
- description: Timestamp when balances were calculated
  name: asOfDate
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-account-balances-schema.json
slug: temenos-transact-core-banking-account-balances
source_filename: temenos-transact-core-banking-account-balances-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountBalances\",\n  \"type\": \"object\",\n  \"description\": \"Balance breakdown for a banking account\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account identifier\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency of the balances\"\n    },\n    \"workingBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Current working balance including pending transactions\"\n    },\n    \"availableBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Balance available for withdrawals and payments\"\n    },\n    \"clearedBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Balance of cleared funds only\"\n    },\n    \"lockedAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount locked or blocked on the account\"\n    },\n    \"overdraftLimit\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Approved overdraft facility amount\"\n    },\n    \"accruedInterest\": {\n      \"type\": \"number\",\n      \"description\": \"Interest accrued but not yet capitalized\"\n    },\n    \"pendingDeposits\": {\n      \"type\": \"number\",\n      \"description\": \"Deposits received but not yet cleared\"\n    },\n    \"asOfDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when balances were calculated\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-account-balances-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: AccountBalances
---
