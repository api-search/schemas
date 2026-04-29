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
source_filename: alpha-vantage-global_quote-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.alphavantage.co/schemas/alpha-vantage-global_quote-schema.json\",\n  \"title\": \"GlobalQuote\",\n  \"type\": \"object\",\n  \"description\": \"Latest real-time stock quote data\",\n  \"properties\": {\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Stock ticker symbol\"\n    },\n    \"open\": {\n      \"type\": \"string\",\n      \"description\": \"Opening price for the day\"\n    },\n    \"high\": {\n      \"type\": \"string\",\n      \"description\": \"Intraday high price\"\n    },\n    \"low\": {\n      \"type\": \"string\",\n      \"description\": \"Intraday low price\"\n    },\n    \"price\": {\n      \"type\": \"string\",\n      \"description\": \"Latest trade price\"\n    },\n    \"volume\": {\n      \"type\": \"string\",\n      \"description\": \"Volume of shares traded\"\n    },\n    \"latestTradingDay\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date\",\n      \"description\": \"Most recent trading day\"\n    },\n    \"previousClose\": {\n      \"type\": \"string\",\n      \"description\": \"Previous day's closing price\"\n    },\n    \"change\": {\n      \"type\": \"string\",\n      \"description\": \"Price change from previous close\"\n    },\n    \"changePercent\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage change from previous close\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/json-schema/alpha-vantage-global_quote-schema.json
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: GlobalQuote
---
