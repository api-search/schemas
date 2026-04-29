---
description: Player wallet balance response.
layout: schema
name: BalanceResponse
properties_list:
- description: Whether the request succeeded.
  name: success
  type: boolean
- description: The player's unique identifier.
  name: playerId
  type: string
- description: Current wallet balance.
  name: balance
  type: number
- description: ISO 4217 three-letter currency code.
  name: currency
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-balance-response-schema.json
slug: wallet-api-balance-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-balance-response-schema.json\",\n  \"title\": \"BalanceResponse\",\n  \"description\": \"Player wallet balance response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the request succeeded.\",\n      \"example\": true\n    },\n    \"playerId\": {\n      \"type\": \"string\",\n      \"description\": \"The player's unique identifier.\",\n      \"example\": \"player-500123\"\n    },\n    \"balance\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Current wallet balance.\",\n      \"example\": 125.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code.\",\n      \"example\": \"USD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-balance-response-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: BalanceResponse
---
