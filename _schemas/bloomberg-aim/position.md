---
description: A position representing holdings of a specific security within a Bloomberg AIM portfolio, including quantity, valuation, and analytics.
layout: schema
name: Position
properties_list:
- description: Unique position identifier
  name: positionId
  type: string
- description: Identifier of the portfolio holding this position
  name: portfolioId
  type: string
- description: Bloomberg ticker of the security held
  name: ticker
  type: string
- description: Full name of the security
  name: securityName
  type: string
- description: FIGI identifier of the security
  name: figi
  type: string
- description: ISIN of the security
  name: isin
  type: string
- description: Asset class of the held security
  name: assetClass
  type: string
- description: Number of shares, contracts, or units held (negative for short positions)
  name: quantity
  type: number
- description: Long or short position
  name: side
  type: string
- description: Total cost basis of the position in local currency
  name: costBasis
  type: number
- description: Average cost per unit
  name: averageCost
  type: number
- description: Current market price per unit
  name: marketPrice
  type: number
- description: Current market value of the position (quantity x market price)
  name: marketValue
  type: number
- description: Market value converted to portfolio base currency
  name: marketValueBase
  type: number
- description: Local trading currency of the security (ISO 4217)
  name: localCurrency
  type: string
- description: Exchange rate from local currency to portfolio base currency
  name: fxRate
  type: number
- description: Position weight as percentage of total portfolio market value
  name: weight
  type: number
- description: Unrealized profit or loss on the position
  name: unrealizedPnL
  type: number
- description: Realized profit or loss from closed portions
  name: realizedPnL
  type: number
- description: Unrealized P&L as a percentage of cost basis
  name: unrealizedPnLPercent
  type: number
- description: Profit or loss for the current trading day
  name: dailyPnL
  type: number
- description: Accrued interest for fixed income positions
  name: accruedInterest
  type: number
- description: Current yield for fixed income positions
  name: yield
  type: number
- description: Modified duration for fixed income positions
  name: duration
  type: number
- description: Convexity for fixed income positions
  name: convexity
  type: number
- description: Credit rating for fixed income positions
  name: creditRating
  type: string
- description: Beta of the security relative to the benchmark
  name: beta
  type: number
- description: Industry sector of the security
  name: sector
  type: string
- description: Country of the security (ISO 3166-1 alpha-2)
  name: country
  type: string
- description: Date the position was initiated or last traded
  name: tradeDate
  type: string
- description: Settlement date for the most recent trade
  name: settleDate
  type: string
- description: Timestamp of the last position update
  name: lastUpdated
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/position.json
slug: position
source_filename: position.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://bloomberg.com/schemas/position.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Position\",\n  \"description\": \"A position representing holdings of a specific security within a Bloomberg AIM portfolio, including quantity, valuation, and analytics.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ticker\",\n    \"quantity\",\n    \"portfolioId\"\n  ],\n  \"properties\": {\n    \"positionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique position identifier\"\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the portfolio holding this position\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg ticker of the security held\",\n      \"examples\": [\n        \"IBM US Equity\",\n        \"AAPL US Equity\"\n      ]\n    },\n    \"securityName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Full name of the security\"\n    },\n    \"figi\": {\n      \"type\": \"string\",\n      \"description\": \"FIGI identifier of the security\",\n      \"pattern\": \"^BBG[A-Z0-9]{9}$\"\n    },\n    \"isin\": {\n      \"type\": \"string\",\n      \"description\": \"ISIN of the security\",\n      \"pattern\": \"^[A-Z]{2}[A-Z0-9]{9}[0-9]$\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class of the held security\",\n      \"enum\": [\n        \"Equity\",\n        \"Fixed Income\",\n        \"Commodity\",\n        \"Currency\",\n        \"Index\",\n        \"Mortgage\",\n        \"Municipal\",\n        \"Preferred\",\n        \"Money Market\",\n        \"Government\",\n        \"Corporate\",\n        \"Option\",\n        \"Future\",\n        \"Fund\",\n        \"ETF\",\n        \"Cash\"\n      ]\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Number of shares, contracts, or units held (negative for short positions)\"\
  \n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\": \"Long or short position\",\n      \"enum\": [\n        \"Long\",\n        \"Short\"\n      ]\n    },\n    \"costBasis\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost basis of the position in local currency\"\n    },\n    \"averageCost\": {\n      \"type\": \"number\",\n      \"description\": \"Average cost per unit\"\n    },\n    \"marketPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Current market price per unit\"\n    },\n    \"marketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Current market value of the position (quantity x market price)\"\n    },\n    \"marketValueBase\": {\n      \"type\": \"number\",\n      \"description\": \"Market value converted to portfolio base currency\"\n    },\n    \"localCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Local trading currency of the security (ISO 4217)\",\n      \"pattern\": \"\
  ^[A-Z]{3}$\"\n    },\n    \"fxRate\": {\n      \"type\": \"number\",\n      \"description\": \"Exchange rate from local currency to portfolio base currency\"\n    },\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Position weight as percentage of total portfolio market value\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"unrealizedPnL\": {\n      \"type\": \"number\",\n      \"description\": \"Unrealized profit or loss on the position\"\n    },\n    \"realizedPnL\": {\n      \"type\": \"number\",\n      \"description\": \"Realized profit or loss from closed portions\"\n    },\n    \"unrealizedPnLPercent\": {\n      \"type\": \"number\",\n      \"description\": \"Unrealized P&L as a percentage of cost basis\"\n    },\n    \"dailyPnL\": {\n      \"type\": \"number\",\n      \"description\": \"Profit or loss for the current trading day\"\n    },\n    \"accruedInterest\": {\n      \"type\": \"number\",\n      \"description\": \"Accrued interest for\
  \ fixed income positions\"\n    },\n    \"yield\": {\n      \"type\": \"number\",\n      \"description\": \"Current yield for fixed income positions\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"Modified duration for fixed income positions\"\n    },\n    \"convexity\": {\n      \"type\": \"number\",\n      \"description\": \"Convexity for fixed income positions\"\n    },\n    \"creditRating\": {\n      \"type\": \"string\",\n      \"description\": \"Credit rating for fixed income positions\",\n      \"examples\": [\n        \"AAA\",\n        \"AA+\",\n        \"BBB-\"\n      ]\n    },\n    \"beta\": {\n      \"type\": \"number\",\n      \"description\": \"Beta of the security relative to the benchmark\"\n    },\n    \"sector\": {\n      \"type\": \"string\",\n      \"description\": \"Industry sector of the security\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of the security (ISO 3166-1 alpha-2)\",\n\
  \      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"tradeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the position was initiated or last traded\"\n    },\n    \"settleDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Settlement date for the most recent trade\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last position update\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/position.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Position
---
