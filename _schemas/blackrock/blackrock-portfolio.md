---
description: Schema for a portfolio record in the BlackRock Aladdin platform
layout: schema
name: BlackRock Aladdin Portfolio
properties_list:
- description: Unique portfolio identifier in Aladdin
  name: portfolioId
  type: string
- description: Display name of the portfolio
  name: portfolioName
  type: string
- description: Base currency (ISO 4217)
  name: currency
  type: string
- description: Total market value of the portfolio in base currency
  name: totalMarketValue
  type: number
- description: Valuation date
  name: asOfDate
  type: string
- description: Benchmark identifier for performance attribution
  name: benchmarkId
  type: string
- description: Portfolio manager identifier
  name: managerId
  type: string
- description: Investment strategy or mandate
  name: strategy
  type: string
- description: Holdings within the portfolio
  name: positions
  type: array
provider_name: BlackRock
provider_slug: blackrock
schema_file: json-schema/blackrock-portfolio-schema.json
slug: blackrock-portfolio
tags:
- Asset Management
- Finance
- FinTech
- Investment Management
- Portfolio Management
- Risk Analytics
title: BlackRock Aladdin Portfolio
---
