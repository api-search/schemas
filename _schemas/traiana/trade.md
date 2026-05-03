---
description: A trade processed through the Traiana Harmony network, representing a cross-asset transaction including FX, equities, equity derivatives, and exchange-traded derivatives.
layout: schema
name: Trade
properties_list:
- description: Unique identifier for the trade within the Harmony network
  name: tradeId
  type: string
- description: External trade reference identifier from the submitting system
  name: externalTradeId
  type: string
- description: Asset class of the traded instrument
  name: assetClass
  type: string
- description: Instrument identifier or symbol
  name: instrument
  type: string
- description: Trade direction
  name: side
  type: string
- description: Trade quantity or notional amount
  name: quantity
  type: number
- description: Execution price
  name: price
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Identifier of the counterparty
  name: counterpartyId
  type: string
- description: Identifier of the executing broker
  name: executingBrokerId
  type: string
- description: Identifier of the prime broker
  name: primeBrokerId
  type: string
- description: Trade execution date
  name: tradeDate
  type: string
- description: Expected settlement date
  name: settlementDate
  type: string
- description: Current processing status of the trade
  name: status
  type: string
- description: Timestamp when the trade was submitted
  name: createdAt
  type: string
- description: Timestamp of the last status update
  name: updatedAt
  type: string
provider_name: Traiana
provider_slug: traiana
schema_file: json-schema/trade.json
slug: trade
source_filename: trade.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/trade.json\",\n  \"title\": \"Trade\",\n  \"description\": \"A trade processed through the Traiana Harmony network, representing a cross-asset transaction including FX, equities, equity derivatives, and exchange-traded derivatives.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tradeId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the trade within the Harmony network\"\n    },\n    \"externalTradeId\": {\n      \"type\": \"string\",\n      \"description\": \"External trade reference identifier from the submitting system\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class of the traded instrument\",\n      \"enum\": [\"FX\", \"Equities\", \"EquityDerivatives\", \"ETD\"]\n    },\n    \"instrument\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Instrument identifier or symbol\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\": \"Trade direction\",\n      \"enum\": [\"Buy\", \"Sell\"]\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Trade quantity or notional amount\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Execution price\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"counterpartyId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the counterparty\"\n    },\n    \"executingBrokerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the executing broker\"\n    },\n    \"primeBrokerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the prime broker\"\n    },\n    \"tradeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n \
  \     \"description\": \"Trade execution date\"\n    },\n    \"settlementDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Expected settlement date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current processing status of the trade\",\n      \"enum\": [\"Pending\", \"Matched\", \"Confirmed\", \"Rejected\", \"Cancelled\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the trade was submitted\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last status update\"\n    }\n  },\n  \"required\": [\"tradeId\", \"assetClass\", \"instrument\", \"side\", \"quantity\", \"price\", \"currency\", \"counterpartyId\", \"tradeDate\", \"status\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/trade.json
tags:
- Fintech
- Foreign Exchange
- Post-Trade Processing
- Risk Management
title: Trade
---
