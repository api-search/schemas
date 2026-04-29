---
description: Response for wallet deposit or withdrawal operations.
layout: schema
name: WalletTransactionResponse
properties_list:
- description: Whether the transaction succeeded.
  name: success
  type: boolean
- description: The transaction identifier.
  name: transactionId
  type: string
- description: Updated wallet balance after the transaction.
  name: balance
  type: number
- description: ISO 4217 three-letter currency code.
  name: currency
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-wallet-transaction-response-schema.json
slug: wallet-api-wallet-transaction-response
source_filename: wallet-api-wallet-transaction-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-wallet-transaction-response-schema.json\",\n  \"title\": \"WalletTransactionResponse\",\n  \"description\": \"Response for wallet deposit or withdrawal operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the transaction succeeded.\",\n      \"example\": true\n    },\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"The transaction identifier.\",\n      \"example\": \"txn-abc123\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Updated wallet balance after the transaction.\",\n      \"example\": 150.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency\
  \ code.\",\n      \"example\": \"USD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-wallet-transaction-response-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: WalletTransactionResponse
---
