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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.alphavantage.co/schemas/alpha-vantage-exchange_rate-schema.json\",\n  \"title\": \"ExchangeRate\",\n  \"type\": \"object\",\n  \"description\": \"Real-time currency exchange rate between two currencies\",\n  \"properties\": {\n    \"fromCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Source currency ISO code\"\n    },\n    \"fromCurrencyName\": {\n      \"type\": \"string\",\n      \"description\": \"Source currency full name\"\n    },\n    \"toCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Destination currency ISO code\"\n    },\n    \"toCurrencyName\": {\n      \"type\": \"string\",\n      \"description\": \"Destination currency full name\"\n    },\n    \"exchangeRate\": {\n      \"type\": \"string\",\n      \"description\": \"Current exchange rate\"\n    },\n    \"lastRefreshed\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Timestamp of last data refresh\"\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone of the refresh timestamp\"\n    },\n    \"bidPrice\": {\n      \"type\": \"string\",\n      \"description\": \"Current bid price\"\n    },\n    \"askPrice\": {\n      \"type\": \"string\",\n      \"description\": \"Current ask price\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/json-schema/alpha-vantage-exchange_rate-schema.json
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: ExchangeRate
---
