---
description: Represents a completed trade execution on the Binance exchange.
layout: schema
name: Binance Trade
properties_list:
- description: Trading pair symbol.
  name: symbol
  type: string
- description: Unique trade identifier.
  name: id
  type: integer
- description: Order ID that generated this trade.
  name: orderId
  type: integer
- description: Order list ID if part of an OCO. -1 otherwise.
  name: orderListId
  type: integer
- description: Trade execution price.
  name: price
  type: string
- description: Trade quantity in base asset.
  name: qty
  type: string
- description: Trade quantity in quote asset.
  name: quoteQty
  type: string
- description: Commission amount charged for this trade.
  name: commission
  type: string
- description: Asset used for commission payment.
  name: commissionAsset
  type: string
- description: Trade execution time in milliseconds since Unix epoch.
  name: time
  type: integer
- description: Whether the account was the buyer in this trade.
  name: isBuyer
  type: boolean
- description: Whether the account was the maker (liquidity provider) in this trade.
  name: isMaker
  type: boolean
- description: Whether this trade was the best price match.
  name: isBestMatch
  type: boolean
- description: Whether the buyer was the maker.
  name: isBuyerMaker
  type: boolean
provider_name: Binance
provider_slug: binance
schema_file: json-schema/binance-trade-schema.json
slug: binance-trade
source_filename: binance-trade-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/binance/trade.json\",\n  \"title\": \"Binance Trade\",\n  \"description\": \"Represents a completed trade execution on the Binance exchange.\",\n  \"type\": \"object\",\n  \"required\": [\"symbol\", \"id\", \"price\", \"qty\", \"time\"],\n  \"properties\": {\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Trading pair symbol.\",\n      \"pattern\": \"^[A-Z0-9]+$\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique trade identifier.\"\n    },\n    \"orderId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Order ID that generated this trade.\"\n    },\n    \"orderListId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Order list ID if part of an OCO. -1 otherwise.\"\n    },\n    \"price\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Trade execution price.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"qty\": {\n      \"type\": \"string\",\n      \"description\": \"Trade quantity in base asset.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"quoteQty\": {\n      \"type\": \"string\",\n      \"description\": \"Trade quantity in quote asset.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"commission\": {\n      \"type\": \"string\",\n      \"description\": \"Commission amount charged for this trade.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"commissionAsset\": {\n      \"type\": \"string\",\n      \"description\": \"Asset used for commission payment.\",\n      \"pattern\": \"^[A-Z0-9]+$\"\n    },\n    \"time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Trade execution time in milliseconds since Unix epoch.\"\n    },\n    \"isBuyer\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether the account was the buyer in this trade.\"\n    },\n    \"isMaker\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account was the maker (liquidity provider) in this trade.\"\n    },\n    \"isBestMatch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this trade was the best price match.\"\n    },\n    \"isBuyerMaker\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the buyer was the maker.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/json-schema/binance-trade-schema.json
tags:
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Finance
- DeFi
- Market Data
title: Binance Trade
---
