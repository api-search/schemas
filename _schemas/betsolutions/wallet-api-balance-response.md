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
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: BalanceResponse
---
