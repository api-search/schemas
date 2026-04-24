---
description: A fill (execution) in the Bloomberg Execution Management System (EMSX) representing a completed or partial trade execution against a route. Fills contain execution price, quantity, broker, exchange, and settlement information.
layout: schema
name: Bloomberg EMSX Fill
properties_list:
- description: Unique fill identifier within the EMSX blotter
  name: fillId
  type: integer
- description: Parent order sequence number
  name: orderSequenceNumber
  type: integer
- description: Parent route identifier
  name: routeId
  type: integer
- description: Bloomberg security ticker symbol
  name: ticker
  type: string
- description: Side of the fill
  name: side
  type: string
- description: Executed quantity in this fill
  name: fillAmount
  type: number
- description: Execution price for this fill
  name: fillPrice
  type: number
- description: Bloomberg broker code of the executing broker
  name: broker
  type: string
- description: Full name of the executing broker
  name: brokerName
  type: string
- description: Exchange or venue where the execution occurred
  name: exchange
  type: string
- description: Trade currency in ISO 4217 three-letter code
  name: currency
  type: string
- description: Settlement date for the trade
  name: settlementDate
  type: string
- description: Trade date (date the execution occurred)
  name: tradeDate
  type: string
- description: ISO 8601 timestamp of the fill execution
  name: fillTime
  type: string
- description: Trading account identifier
  name: account
  type: string
- description: Whether this fill was manually entered (e.g., for voice-brokered trades)
  name: isManual
  type: boolean
- description: Counterparty identifier for the trade
  name: contraParty
  type: string
provider_name: Bloomberg EMSX
provider_slug: bloomberg-emsx
schema_file: json-schema/bloomberg-emsx-fill-schema.json
slug: bloomberg-emsx-fill
tags:
- Bloomberg
- Execution Management
- Financial Services
- Order Management
- Trading
title: Bloomberg EMSX Fill
---
