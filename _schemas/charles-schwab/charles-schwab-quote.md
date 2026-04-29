---
description: ''
layout: schema
name: Schwab Quote
properties_list:
- description: ''
  name: symbol
  type: string
- description: ''
  name: bidPrice
  type: number
- description: ''
  name: askPrice
  type: number
- description: ''
  name: lastPrice
  type: number
- description: ''
  name: openPrice
  type: number
- description: ''
  name: highPrice
  type: number
- description: ''
  name: lowPrice
  type: number
- description: ''
  name: netChange
  type: number
- description: ''
  name: totalVolume
  type: integer
- description: ''
  name: quoteTime
  type: integer
- description: ''
  name: tradeTime
  type: integer
provider_name: Charles Schwab
provider_slug: charles-schwab
schema_file: json-schema/charles-schwab-quote-schema.json
slug: charles-schwab-quote
source_filename: charles-schwab-quote-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.schwab.com/schemas/quote.json\",\n  \"title\": \"Schwab Quote\",\n  \"type\": \"object\",\n  \"required\": [\"symbol\"],\n  \"properties\": {\n    \"symbol\": { \"type\": \"string\" },\n    \"bidPrice\": { \"type\": \"number\" },\n    \"askPrice\": { \"type\": \"number\" },\n    \"lastPrice\": { \"type\": \"number\" },\n    \"openPrice\": { \"type\": \"number\" },\n    \"highPrice\": { \"type\": \"number\" },\n    \"lowPrice\": { \"type\": \"number\" },\n    \"netChange\": { \"type\": \"number\" },\n    \"totalVolume\": { \"type\": \"integer\" },\n    \"quoteTime\": { \"type\": \"integer\" },\n    \"tradeTime\": { \"type\": \"integer\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/json-schema/charles-schwab-quote-schema.json
tags:
- Accounts
- Banking
- Brokerage
- Financial Services
- Investing
- Market Data
- OAuth 2.0
- Orders
- Trading
title: Schwab Quote
---
