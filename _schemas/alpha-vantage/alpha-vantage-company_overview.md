---
description: Company fundamental data including financial ratios and business description
layout: schema
name: CompanyOverview
properties_list:
- description: Stock ticker symbol
  name: Symbol
  type: string
- description: Company name
  name: Name
  type: string
- description: Company business description
  name: Description
  type: string
- description: Stock exchange listing
  name: Exchange
  type: string
- description: Trading currency code
  name: Currency
  type: string
- description: Country of incorporation
  name: Country
  type: string
- description: Business sector
  name: Sector
  type: string
- description: Industry classification
  name: Industry
  type: string
- description: Total market capitalization in USD
  name: MarketCapitalization
  type: string
- description: Price-to-earnings ratio
  name: PERatio
  type: string
- description: Earnings per share (TTM)
  name: EPS
  type: string
- description: Annual dividend yield as decimal
  name: DividendYield
  type: string
- description: Beta coefficient relative to S&P 500
  name: Beta
  type: string
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-company_overview-schema.json
slug: alpha-vantage-company_overview
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: CompanyOverview
---
