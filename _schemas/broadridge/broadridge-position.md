---
description: JSON Schema for a Broadridge Wealth Management securities position (holding) in a brokerage account.
layout: schema
name: Broadridge Position
properties_list:
- description: Unique position identifier
  name: positionId
  type: string
- description: Brokerage account number
  name: accountNumber
  type: string
- description: Committee on Uniform Securities Identification Procedures number
  name: cusip
  type: string
- description: Ticker symbol
  name: symbol
  type: string
- description: Full security name/description
  name: securityDescription
  type: string
- description: ''
  name: assetClass
  type: string
- description: Number of shares or units held
  name: quantity
  type: number
- description: Current price per share/unit
  name: price
  type: number
- description: Total market value (quantity * price)
  name: marketValue
  type: number
- description: Total cost basis for the position
  name: costBasis
  type: number
- description: Unrealized gain/loss (marketValue - costBasis)
  name: unrealizedGainLoss
  type: number
- description: Unrealized gain/loss as percentage of cost basis
  name: unrealizedGainLossPct
  type: number
- description: ''
  name: currency
  type: string
- description: Date the position data is as-of
  name: asOfDate
  type: string
provider_name: broadridge
provider_slug: broadridge
schema_file: json-schema/broadridge-position-schema.json
slug: broadridge-position
tags: []
title: Broadridge Position
---
