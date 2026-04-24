---
description: Represents a completed trade execution on the Binance exchange.
layout: schema
name: Binance Trade
properties_list:
- description: Trading pair symbol.
  name: symbol
  type: string
- description: Unique trade identifier.
  name: id
  type: integer
- description: Order ID that generated this trade.
  name: orderId
  type: integer
- description: Order list ID if part of an OCO. -1 otherwise.
  name: orderListId
  type: integer
- description: Trade execution price.
  name: price
  type: string
- description: Trade quantity in base asset.
  name: qty
  type: string
- description: Trade quantity in quote asset.
  name: quoteQty
  type: string
- description: Commission amount charged for this trade.
  name: commission
  type: string
- description: Asset used for commission payment.
  name: commissionAsset
  type: string
- description: Trade execution time in milliseconds since Unix epoch.
  name: time
  type: integer
- description: Whether the account was the buyer in this trade.
  name: isBuyer
  type: boolean
- description: Whether the account was the maker (liquidity provider) in this trade.
  name: isMaker
  type: boolean
- description: Whether this trade was the best price match.
  name: isBestMatch
  type: boolean
- description: Whether the buyer was the maker.
  name: isBuyerMaker
  type: boolean
provider_name: Binance
provider_slug: binance
schema_file: json-schema/binance-trade-schema.json
slug: binance-trade
tags:
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Finance
- DeFi
- Market Data
title: Binance Trade
---
