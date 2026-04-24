---
description: A trading order representing an instruction to buy or sell a financial instrument, supporting various order types, time-in-force options, and algorithmic execution strategies for institutional buy-side trading.
layout: schema
name: Bloomberg Buyside Order
properties_list:
- description: Unique order identifier
  name: id
  type: string
- description: Bloomberg security identifier (e.g., 'AAPL US Equity')
  name: security
  type: string
- description: Human-readable security name
  name: securityName
  type: string
- description: Order side indicating the direction of the trade
  name: side
  type: string
- description: Order type determining execution behavior
  name: orderType
  type: string
- description: Total order quantity in shares or units
  name: quantity
  type: number
- description: Cumulative filled quantity
  name: filledQuantity
  type: number
- description: Remaining quantity to be filled
  name: remainingQuantity
  type: number
- description: Limit price for LIMIT and STOP_LIMIT orders
  name: limitPrice
  type: number
- description: Stop trigger price for STOP and STOP_LIMIT orders
  name: stopPrice
  type: number
- description: Volume-weighted average price of all fills
  name: averageFillPrice
  type: number
- description: Current order lifecycle status
  name: status
  type: string
- description: Time-in-force instruction governing order duration
  name: timeInForce
  type: string
- description: Expiration date for Good-Till-Date (GTD) orders
  name: expirationDate
  type: string
- description: Target portfolio for post-trade allocation
  name: portfolioId
  type: string
- description: Broker identifier for order routing
  name: brokerId
  type: string
- description: Algorithmic execution strategy name
  name: algorithm
  type: string
- description: Algorithm-specific execution parameters
  name: algorithmParams
  type: object
- description: Order currency (ISO 4217)
  name: currency
  type: string
- description: Identifier of the trader who placed the order
  name: trader
  type: string
- description: Execution reports (fills) for this order
  name: executions
  type: array
- description: Order creation timestamp
  name: createdAt
  type: string
- description: Most recent order update timestamp
  name: updatedAt
  type: string
provider_name: Bloomberg Buyside Enterprise Solutions
provider_slug: bloomberg-buyside-enterprise-solutions
schema_file: json-schema/bloomberg-buyside-order-schema.json
slug: bloomberg-buyside-order
tags:
- Analytics
- Asset Management
- Buy-Side
- Enterprise Solutions
- Financial Services
- Market Data
- Portfolio Management
- Trading
title: Bloomberg Buyside Order
---
