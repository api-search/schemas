---
description: Request body for retrieving a player's wallet balance.
layout: schema
name: BalanceRequest
properties_list:
- description: The merchant's unique identifier.
  name: merchantId
  type: string
- description: The player's unique identifier.
  name: playerId
  type: string
- description: SHA-256 hash for request authentication.
  name: hash
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-balance-request-schema.json
slug: wallet-api-balance-request
source_filename: wallet-api-balance-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-balance-request-schema.json\",\n  \"title\": \"BalanceRequest\",\n  \"description\": \"Request body for retrieving a player's wallet balance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantId\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's unique identifier.\",\n      \"example\": \"merchant-001\"\n    },\n    \"playerId\": {\n      \"type\": \"string\",\n      \"description\": \"The player's unique identifier.\",\n      \"example\": \"player-500123\"\n    },\n    \"hash\": {\n      \"type\": \"string\",\n      \"description\": \"SHA-256 hash for request authentication.\",\n      \"example\": \"c3d4e5f6...\"\n    }\n  },\n  \"required\": [\n    \"merchantId\",\n    \"playerId\",\n    \"hash\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-balance-request-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: BalanceRequest
---
