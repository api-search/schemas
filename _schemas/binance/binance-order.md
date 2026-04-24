---
description: Represents a trading order on the Binance exchange, applicable across spot, margin, and futures markets.
layout: schema
name: Binance Order
properties_list:
- description: Trading pair symbol, e.g. BTCUSDT.
  name: symbol
  type: string
- description: Unique order identifier assigned by Binance.
  name: orderId
  type: integer
- description: Order list identifier for OCO orders. -1 if not part of an OCO.
  name: orderListId
  type: integer
- description: Client-specified unique order identifier.
  name: clientOrderId
  type: string
- description: Order price as a decimal string.
  name: price
  type: string
- description: Original order quantity.
  name: origQty
  type: string
- description: Quantity that has been executed/filled.
  name: executedQty
  type: string
- description: Cumulative quote asset quantity transacted.
  name: cummulativeQuoteQty
  type: string
- description: Current order status.
  name: status
  type: string
- description: Time in force policy.
  name: timeInForce
  type: string
- description: Order type.
  name: type
  type: string
- description: 'Order side: buy or sell.'
  name: side
  type: string
- description: Stop/trigger price for conditional orders.
  name: stopPrice
  type: string
- description: Iceberg quantity for iceberg orders.
  name: icebergQty
  type: string
- description: Order creation time in milliseconds since Unix epoch.
  name: time
  type: integer
- description: Last update time in milliseconds since Unix epoch.
  name: updateTime
  type: integer
- description: Whether the order is currently on the order book.
  name: isWorking
  type: boolean
- description: Time when the order started working on the book.
  name: workingTime
  type: integer
- description: Original quote order quantity for market orders.
  name: origQuoteOrderQty
  type: string
- description: Self-trade prevention mode.
  name: selfTradePreventionMode
  type: string
- description: Position side for futures hedge mode.
  name: positionSide
  type: string
- description: Whether this is a reduce-only order (futures).
  name: reduceOnly
  type: boolean
- description: Whether this order closes the entire position (futures).
  name: closePosition
  type: boolean
- description: Activation price for trailing stop market orders.
  name: activatePrice
  type: string
- description: Callback rate for trailing stop market orders.
  name: priceRate
  type: string
- description: Stop price trigger type for futures.
  name: workingType
  type: string
- description: Whether price protection is enabled.
  name: priceProtect
  type: boolean
provider_name: Binance
provider_slug: binance
schema_file: json-schema/binance-order-schema.json
slug: binance-order
tags:
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Finance
- DeFi
- Market Data
title: Binance Order
---
