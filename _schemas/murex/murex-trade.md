---
description: Represents a financial trade executed on the Murex MX.3 platform across any supported asset class including derivatives, fixed income, equities, FX, and commodities.
layout: schema
name: Murex Trade
properties_list:
- description: Unique trade identifier assigned by MX.3
  name: tradeId
  type: string
- description: External trade reference from a connected system
  name: externalTradeId
  type: string
- description: Associated order identifier if the trade originated from an order
  name: orderId
  type: string
- description: Current trade lifecycle status
  name: status
  type: string
- description: Trade side from the perspective of the booking entity
  name: side
  type: string
- description: Asset class classification of the traded instrument
  name: assetClass
  type: string
- description: MX.3 instrument identifier
  name: instrumentId
  type: string
- description: Instrument display name
  name: instrumentName
  type: string
- description: Specific instrument type (e.g., IRS, CDS, FXForward, Bond, Option)
  name: instrumentType
  type: string
- description: Trade quantity, notional amount, or number of contracts
  name: quantity
  type: number
- description: Trade execution price, rate, or spread
  name: price
  type: number
- description: Primary trade currency in ISO 4217 format
  name: currency
  type: string
- description: Secondary currency for FX and cross-currency instruments
  name: secondaryCurrency
  type: string
- description: Portfolio or book where the trade is booked
  name: portfolioId
  type: string
- description: Portfolio display name
  name: portfolioName
  type: string
- description: Trading desk identifier
  name: deskId
  type: string
- description: ''
  name: counterparty
  type: object
- description: Trade execution date
  name: tradeDate
  type: string
- description: Settlement or value date
  name: valueDate
  type: string
- description: Maturity or expiry date for term instruments
  name: maturityDate
  type: string
- description: Legal entity that is party to the trade
  name: entity
  type: string
- description: Trader who executed the trade
  name: trader
  type: string
- description: Sales person associated with the trade
  name: salesPerson
  type: string
- description: International Securities Identification Number
  name: isin
  type: string
- description: Unique Transaction Identifier for regulatory reporting
  name: uti
  type: string
- description: Trade creation timestamp in MX.3
  name: createdAt
  type: string
- description: Last modification timestamp
  name: updatedAt
  type: string
provider_name: Murex
provider_slug: murex
schema_file: json-schema/murex-trade-schema.json
slug: murex-trade
source_filename: murex-trade-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.murex.com/schemas/murex/trade.json\",\n  \"title\": \"Murex Trade\",\n  \"description\": \"Represents a financial trade executed on the Murex MX.3 platform across any supported asset class including derivatives, fixed income, equities, FX, and commodities.\",\n  \"type\": \"object\",\n  \"required\": [\"tradeId\", \"side\", \"assetClass\", \"instrumentId\", \"quantity\", \"price\", \"currency\", \"portfolioId\", \"tradeDate\"],\n  \"properties\": {\n    \"tradeId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique trade identifier assigned by MX.3\"\n    },\n    \"externalTradeId\": {\n      \"type\": \"string\",\n      \"description\": \"External trade reference from a connected system\"\n    },\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated order identifier if the trade originated from an order\"\n    },\n    \"status\": {\n\
  \      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Amended\", \"Cancelled\", \"Matured\", \"Terminated\"],\n      \"description\": \"Current trade lifecycle status\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"enum\": [\"Buy\", \"Sell\"],\n      \"description\": \"Trade side from the perspective of the booking entity\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"enum\": [\"FX\", \"IRD\", \"Equity\", \"Credit\", \"Commodity\", \"FixedIncome\"],\n      \"description\": \"Asset class classification of the traded instrument\"\n    },\n    \"instrumentId\": {\n      \"type\": \"string\",\n      \"description\": \"MX.3 instrument identifier\"\n    },\n    \"instrumentName\": {\n      \"type\": \"string\",\n      \"description\": \"Instrument display name\"\n    },\n    \"instrumentType\": {\n      \"type\": \"string\",\n      \"description\": \"Specific instrument type (e.g., IRS, CDS, FXForward, Bond, Option)\"\n    },\n    \"quantity\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Trade quantity, notional amount, or number of contracts\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Trade execution price, rate, or spread\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"Primary trade currency in ISO 4217 format\"\n    },\n    \"secondaryCurrency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"Secondary currency for FX and cross-currency instruments\"\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio or book where the trade is booked\"\n    },\n    \"portfolioName\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio display name\"\n    },\n    \"deskId\": {\n      \"type\": \"string\",\n      \"description\": \"Trading desk identifier\"\n    },\n    \"counterparty\": {\n      \"$ref\": \"#/$defs/Counterparty\"\
  \n    },\n    \"tradeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Trade execution date\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Settlement or value date\"\n    },\n    \"maturityDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Maturity or expiry date for term instruments\"\n    },\n    \"entity\": {\n      \"type\": \"string\",\n      \"description\": \"Legal entity that is party to the trade\"\n    },\n    \"trader\": {\n      \"type\": \"string\",\n      \"description\": \"Trader who executed the trade\"\n    },\n    \"salesPerson\": {\n      \"type\": \"string\",\n      \"description\": \"Sales person associated with the trade\"\n    },\n    \"isin\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{2}[A-Z0-9]{9}[0-9]$\",\n      \"description\": \"International Securities Identification Number\"\n    },\n\
  \    \"uti\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Transaction Identifier for regulatory reporting\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Trade creation timestamp in MX.3\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  },\n  \"$defs\": {\n    \"Counterparty\": {\n      \"type\": \"object\",\n      \"description\": \"Counterparty to the trade\",\n      \"properties\": {\n        \"counterpartyId\": {\n          \"type\": \"string\",\n          \"description\": \"Counterparty unique identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Counterparty legal name\"\n        },\n        \"lei\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z0-9]{20}$\",\n          \"description\": \"Legal Entity Identifier\"\
  \n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Counterparty domicile country code\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/murex/refs/heads/main/json-schema/murex-trade-schema.json
tags:
- Capital Markets
- Enterprise Software
- Financial Services
- Fintech
- Risk Management
- Trading
title: Murex Trade
---
