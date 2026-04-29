---
description: Request body for depositing funds to a player's wallet.
layout: schema
name: DepositRequest
properties_list:
- description: The merchant's unique identifier.
  name: merchantId
  type: string
- description: The player's unique identifier.
  name: playerId
  type: string
- description: Amount to deposit in the player's currency.
  name: amount
  type: number
- description: ISO 4217 three-letter currency code.
  name: currency
  type: string
- description: Unique transaction identifier to prevent duplicate processing.
  name: transactionId
  type: string
- description: SHA-256 hash for request authentication.
  name: hash
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-deposit-request-schema.json
slug: wallet-api-deposit-request
source_filename: wallet-api-deposit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-deposit-request-schema.json\",\n  \"title\": \"DepositRequest\",\n  \"description\": \"Request body for depositing funds to a player's wallet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantId\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's unique identifier.\",\n      \"example\": \"merchant-001\"\n    },\n    \"playerId\": {\n      \"type\": \"string\",\n      \"description\": \"The player's unique identifier.\",\n      \"example\": \"player-500123\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Amount to deposit in the player's currency.\",\n      \"example\": 50.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code.\"\
  ,\n      \"example\": \"USD\"\n    },\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier to prevent duplicate processing.\",\n      \"example\": \"txn-abc123\"\n    },\n    \"hash\": {\n      \"type\": \"string\",\n      \"description\": \"SHA-256 hash for request authentication.\",\n      \"example\": \"a1b2c3d4...\"\n    }\n  },\n  \"required\": [\n    \"merchantId\",\n    \"playerId\",\n    \"amount\",\n    \"currency\",\n    \"transactionId\",\n    \"hash\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-deposit-request-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: DepositRequest
---
