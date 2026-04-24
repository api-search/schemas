---
description: Represents a Binance user account with balances, permissions, and commission rates.
layout: schema
name: Binance Account
properties_list:
- description: Maker commission rate in basis points.
  name: makerCommission
  type: integer
- description: Taker commission rate in basis points.
  name: takerCommission
  type: integer
- description: Buyer commission rate in basis points.
  name: buyerCommission
  type: integer
- description: Seller commission rate in basis points.
  name: sellerCommission
  type: integer
- description: Detailed commission rate structure.
  name: commissionRates
  type: object
- description: Whether the account has trading permission.
  name: canTrade
  type: boolean
- description: Whether the account has withdrawal permission.
  name: canWithdraw
  type: boolean
- description: Whether the account has deposit permission.
  name: canDeposit
  type: boolean
- description: Whether this is a brokered account.
  name: brokered
  type: boolean
- description: Whether self-trade prevention is required.
  name: requireSelfTradePrevention
  type: boolean
- description: Whether Smart Order Routing is prevented.
  name: preventSor
  type: boolean
- description: Last account update time in milliseconds since epoch.
  name: updateTime
  type: integer
- description: Account type identifier.
  name: accountType
  type: string
- description: List of asset balances in the account.
  name: balances
  type: array
- description: Account permission types.
  name: permissions
  type: array
- description: Unique user identifier.
  name: uid
  type: integer
provider_name: Binance
provider_slug: binance
schema_file: json-schema/binance-account-schema.json
slug: binance-account
tags:
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Finance
- DeFi
- Market Data
title: Binance Account
---
