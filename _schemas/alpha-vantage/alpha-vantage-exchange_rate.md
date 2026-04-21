---
description: Real-time currency exchange rate between two currencies
layout: schema
name: ExchangeRate
properties_list:
- description: Source currency ISO code
  name: fromCurrencyCode
  type: string
- description: Source currency full name
  name: fromCurrencyName
  type: string
- description: Destination currency ISO code
  name: toCurrencyCode
  type: string
- description: Destination currency full name
  name: toCurrencyName
  type: string
- description: Current exchange rate
  name: exchangeRate
  type: string
- description: Timestamp of last data refresh
  name: lastRefreshed
  type: string
- description: Time zone of the refresh timestamp
  name: timeZone
  type: string
- description: Current bid price
  name: bidPrice
  type: string
- description: Current ask price
  name: askPrice
  type: string
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-exchange_rate-schema.json
slug: alpha-vantage-exchange_rate
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: ExchangeRate
---
