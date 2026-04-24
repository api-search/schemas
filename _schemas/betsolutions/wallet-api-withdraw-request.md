---
description: Request body for withdrawing funds from a player's wallet.
layout: schema
name: WithdrawRequest
properties_list:
- description: The merchant's unique identifier.
  name: merchantId
  type: string
- description: The player's unique identifier.
  name: playerId
  type: string
- description: Amount to withdraw in the player's currency.
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
schema_file: json-schema/wallet-api-withdraw-request-schema.json
slug: wallet-api-withdraw-request
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: WithdrawRequest
---
