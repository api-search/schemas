---
description: A trading order in the Bloomberg Execution Management System (EMSX) blotter representing an intent to buy or sell a financial instrument. Orders contain instrument details, quantity, pricing instructions, and lifecycle status, and may have one or more routes to brokers for execution.
layout: schema
name: Bloomberg EMSX Order
properties_list:
- description: EMSX order sequence number, the unique identifier for the order within the blotter
  name: sequenceNumber
  type: integer
- description: Bloomberg security ticker symbol identifying the instrument to trade
  name: ticker
  type: string
- description: Order side indicating the direction of the trade
  name: side
  type: string
- description: Total order quantity in shares, contracts, or face value
  name: amount
  type: number
- description: Order type specifying pricing and execution behavior
  name: orderType
  type: string
- description: Limit price for limit orders (LMT, STP_LMT, LOC)
  name: limitPrice
  type: number
- description: Stop trigger price for stop orders (STP, STP_LMT)
  name: stopPrice
  type: number
- description: Time in force instruction governing how long the order remains active
  name: timeInForce
  type: string
- description: Expiration date for GTD (Good Till Date) orders
  name: goodTillDate
  type: string
- description: Current lifecycle status of the order
  name: status
  type: string
- description: Total quantity filled across all routes
  name: filledAmount
  type: number
- description: Volume-weighted average fill price across all executions
  name: averagePrice
  type: number
- description: Remaining unfilled quantity (amount minus filledAmount)
  name: remainingAmount
  type: number
- description: Asset class of the instrument being traded
  name: assetClass
  type: string
- description: Primary exchange or marketplace for the instrument
  name: exchange
  type: string
- description: Trading currency in ISO 4217 three-letter code
  name: currency
  type: string
- description: Trading account identifier for allocation
  name: account
  type: string
- description: Free-text notes attached to the order by the trader
  name: notes
  type: string
- description: Name of the trader who created the order
  name: traderName
  type: string
- description: ISO 8601 timestamp when the order was created
  name: createdTime
  type: string
- description: ISO 8601 timestamp when the order was last modified
  name: lastModifiedTime
  type: string
- description: Summary of routes associated with this order
  name: routes
  type: array
- description: Custom user-defined fields configured in the EMSX blotter
  name: customFields
  type: object
provider_name: Bloomberg EMSX
provider_slug: bloomberg-emsx
schema_file: json-schema/bloomberg-emsx-order-schema.json
slug: bloomberg-emsx-order
tags:
- Bloomberg
- Execution Management
- Financial Services
- Order Management
- Trading
title: Bloomberg EMSX Order
---
