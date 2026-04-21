---
description: Latest real-time stock quote data
layout: schema
name: GlobalQuote
properties_list:
- description: Stock ticker symbol
  name: symbol
  type: string
- description: Opening price for the day
  name: open
  type: string
- description: Intraday high price
  name: high
  type: string
- description: Intraday low price
  name: low
  type: string
- description: Latest trade price
  name: price
  type: string
- description: Volume of shares traded
  name: volume
  type: string
- description: Most recent trading day
  name: latestTradingDay
  type: string
- description: Previous day's closing price
  name: previousClose
  type: string
- description: Price change from previous close
  name: change
  type: string
- description: Percentage change from previous close
  name: changePercent
  type: string
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-global_quote-schema.json
slug: alpha-vantage-global_quote
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: GlobalQuote
---
