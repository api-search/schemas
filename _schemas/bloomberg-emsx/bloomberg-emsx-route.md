---
description: A route in the Bloomberg Execution Management System (EMSX) representing the assignment of an order (or portion thereof) to a specific broker for execution. Routes contain broker details, execution strategy, pricing instructions, and fill status.
layout: schema
name: Bloomberg EMSX Route
properties_list:
- description: EMSX route identifier, unique within the blotter
  name: routeId
  type: integer
- description: Parent order sequence number linking this route to its order
  name: orderSequenceNumber
  type: integer
- description: Bloomberg security ticker symbol
  name: ticker
  type: string
- description: Route side, inherited from the parent order
  name: side
  type: string
- description: Quantity assigned to this route
  name: amount
  type: number
- description: Quantity filled on this route
  name: filledAmount
  type: number
- description: Volume-weighted average fill price on this route
  name: averagePrice
  type: number
- description: Remaining unfilled quantity on this route
  name: remainingAmount
  type: number
- description: Bloomberg broker code identifying the executing broker
  name: broker
  type: string
- description: Full name of the executing broker
  name: brokerName
  type: string
- description: Execution strategy name (e.g., VWAP, TWAP, DMA, Iceberg)
  name: strategy
  type: string
- description: Strategy-specific configurable parameters
  name: strategyParameters
  type: object
- description: Current lifecycle status of the route
  name: status
  type: string
- description: Limit price for the route
  name: limitPrice
  type: number
- description: Order type on the route
  name: orderType
  type: string
- description: Time in force on the route
  name: timeInForce
  type: string
- description: Trading account identifier
  name: account
  type: string
- description: Destination exchange or marketplace
  name: exchange
  type: string
- description: Rejection or cancellation reason code from the broker
  name: reasonCode
  type: string
- description: Human-readable reason for rejection or cancellation
  name: reasonDescription
  type: string
- description: ISO 8601 timestamp when the route was created
  name: createdTime
  type: string
- description: ISO 8601 timestamp when the route was last modified
  name: lastModifiedTime
  type: string
- description: ISO 8601 timestamp of the most recent fill on this route
  name: lastFillTime
  type: string
- description: Custom user-defined fields
  name: customFields
  type: object
provider_name: Bloomberg EMSX
provider_slug: bloomberg-emsx
schema_file: json-schema/bloomberg-emsx-route-schema.json
slug: bloomberg-emsx-route
tags:
- Bloomberg
- Execution Management
- Financial Services
- Order Management
- Trading
title: Bloomberg EMSX Route
---
