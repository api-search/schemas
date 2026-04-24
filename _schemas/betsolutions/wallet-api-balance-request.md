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
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: BalanceRequest
---
