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
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: WalletTransactionResponse
---
