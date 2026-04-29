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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.alphavantage.co/schemas/alpha-vantage-time_series_data-schema.json\",\n  \"title\": \"TimeSeriesData\",\n  \"type\": \"object\",\n  \"description\": \"Stock OHLCV time series data point\",\n  \"properties\": {\n    \"open\": {\n      \"type\": \"string\",\n      \"description\": \"Opening price for the period\"\n    },\n    \"high\": {\n      \"type\": \"string\",\n      \"description\": \"Highest price for the period\"\n    },\n    \"low\": {\n      \"type\": \"string\",\n      \"description\": \"Lowest price for the period\"\n    },\n    \"close\": {\n      \"type\": \"string\",\n      \"description\": \"Closing price for the period\"\n    },\n    \"volume\": {\n      \"type\": \"string\",\n      \"description\": \"Trading volume for the period\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/json-schema/alpha-vantage-time_series_data-schema.json
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: TimeSeriesData
---
