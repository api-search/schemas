---
description: Stock OHLCV time series data point
layout: schema
name: TimeSeriesData
properties_list:
- description: Opening price for the period
  name: open
  type: string
- description: Highest price for the period
  name: high
  type: string
- description: Lowest price for the period
  name: low
  type: string
- description: Closing price for the period
  name: close
  type: string
- description: Trading volume for the period
  name: volume
  type: string
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-time_series_data-schema.json
slug: alpha-vantage-time_series_data
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: TimeSeriesData
---
