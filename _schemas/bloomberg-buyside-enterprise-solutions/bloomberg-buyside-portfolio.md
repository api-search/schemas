---
description: A portfolio represents a collection of financial instrument holdings managed as a single entity for buy-side investment management, including trading portfolios, model portfolios, benchmarks, and composites.
layout: schema
name: Bloomberg Buyside Portfolio
properties_list:
- description: Unique portfolio identifier
  name: id
  type: string
- description: Portfolio name
  name: name
  type: string
- description: Portfolio description
  name: description
  type: string
- description: Portfolio type classification
  name: type
  type: string
- description: Current portfolio status
  name: status
  type: string
- description: Base currency for the portfolio (ISO 4217)
  name: currency
  type: string
- description: Identifier of the assigned benchmark for performance comparison
  name: benchmarkId
  type: string
- description: Portfolio manager identifier
  name: manager
  type: string
- description: Date the portfolio was established
  name: inceptionDate
  type: string
- description: Total current market value of the portfolio in base currency
  name: totalMarketValue
  type: number
- description: Number of distinct holdings in the portfolio
  name: holdingsCount
  type: integer
- description: Current portfolio holdings
  name: holdings
  type: array
- description: Timestamp when the portfolio was created
  name: createdAt
  type: string
- description: Timestamp of the most recent portfolio update
  name: updatedAt
  type: string
provider_name: Bloomberg Buyside Enterprise Solutions
provider_slug: bloomberg-buyside-enterprise-solutions
schema_file: json-schema/bloomberg-buyside-portfolio-schema.json
slug: bloomberg-buyside-portfolio
tags:
- Analytics
- Asset Management
- Buy-Side
- Enterprise Solutions
- Financial Services
- Market Data
- Portfolio Management
- Trading
title: Bloomberg Buyside Portfolio
---
