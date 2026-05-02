---
description: Represents a portfolio position in the Murex MX.3 platform, including market value, P&L, and risk attributes for a specific instrument holding within a portfolio or book.
layout: schema
name: Murex Position
properties_list:
- description: Unique position identifier
  name: positionId
  type: string
- description: Portfolio or book identifier where the position is held
  name: portfolioId
  type: string
- description: Portfolio display name
  name: portfolioName
  type: string
- description: Trading desk identifier
  name: deskId
  type: string
- description: Trading desk display name
  name: deskName
  type: string
- description: MX.3 instrument identifier
  name: instrumentId
  type: string
- description: Instrument display name
  name: instrumentName
  type: string
- description: Asset class classification
  name: assetClass
  type: string
- description: Specific instrument type
  name: instrumentType
  type: string
- description: Position quantity, notional amount, or number of contracts
  name: quantity
  type: number
- description: Current mark-to-market value of the position
  name: marketValue
  type: number
- description: Average cost basis of the position
  name: averageCost
  type: number
- description: Unrealized profit or loss
  name: unrealizedPnL
  type: number
- description: Cumulative realized profit or loss
  name: realizedPnL
  type: number
- description: Accrued interest for fixed income positions
  name: accruedInterest
  type: number
- description: Position currency in ISO 4217 format
  name: currency
  type: string
- description: ''
  name: counterparty
  type: object
- description: Original trade date
  name: tradeDate
  type: string
- description: Value or settlement date
  name: valueDate
  type: string
- description: Maturity or expiry date
  name: maturityDate
  type: string
- description: Position valuation date
  name: asOfDate
  type: string
- description: Legal entity holding the position
  name: entity
  type: string
- description: ''
  name: riskMeasures
  type: object
provider_name: Murex
provider_slug: murex
schema_file: json-schema/murex-position-schema.json
slug: murex-position
source_filename: murex-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.murex.com/schemas/murex/position.json\",\n  \"title\": \"Murex Position\",\n  \"description\": \"Represents a portfolio position in the Murex MX.3 platform, including market value, P&L, and risk attributes for a specific instrument holding within a portfolio or book.\",\n  \"type\": \"object\",\n  \"required\": [\"positionId\", \"portfolioId\", \"instrumentId\", \"quantity\", \"currency\", \"asOfDate\"],\n  \"properties\": {\n    \"positionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique position identifier\"\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio or book identifier where the position is held\"\n    },\n    \"portfolioName\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio display name\"\n    },\n    \"deskId\": {\n      \"type\": \"string\",\n      \"description\": \"Trading desk identifier\"\
  \n    },\n    \"deskName\": {\n      \"type\": \"string\",\n      \"description\": \"Trading desk display name\"\n    },\n    \"instrumentId\": {\n      \"type\": \"string\",\n      \"description\": \"MX.3 instrument identifier\"\n    },\n    \"instrumentName\": {\n      \"type\": \"string\",\n      \"description\": \"Instrument display name\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"enum\": [\"FX\", \"IRD\", \"Equity\", \"Credit\", \"Commodity\", \"FixedIncome\"],\n      \"description\": \"Asset class classification\"\n    },\n    \"instrumentType\": {\n      \"type\": \"string\",\n      \"description\": \"Specific instrument type\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Position quantity, notional amount, or number of contracts\"\n    },\n    \"marketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Current mark-to-market value of the position\"\n    },\n    \"averageCost\": {\n      \"type\": \"\
  number\",\n      \"description\": \"Average cost basis of the position\"\n    },\n    \"unrealizedPnL\": {\n      \"type\": \"number\",\n      \"description\": \"Unrealized profit or loss\"\n    },\n    \"realizedPnL\": {\n      \"type\": \"number\",\n      \"description\": \"Cumulative realized profit or loss\"\n    },\n    \"accruedInterest\": {\n      \"type\": \"number\",\n      \"description\": \"Accrued interest for fixed income positions\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"Position currency in ISO 4217 format\"\n    },\n    \"counterparty\": {\n      \"$ref\": \"#/$defs/Counterparty\"\n    },\n    \"tradeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Original trade date\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Value or settlement date\"\n    },\n    \"maturityDate\": {\n   \
  \   \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Maturity or expiry date\"\n    },\n    \"asOfDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Position valuation date\"\n    },\n    \"entity\": {\n      \"type\": \"string\",\n      \"description\": \"Legal entity holding the position\"\n    },\n    \"riskMeasures\": {\n      \"$ref\": \"#/$defs/RiskMeasures\"\n    }\n  },\n  \"$defs\": {\n    \"Counterparty\": {\n      \"type\": \"object\",\n      \"description\": \"Counterparty to the position\",\n      \"properties\": {\n        \"counterpartyId\": {\n          \"type\": \"string\",\n          \"description\": \"Counterparty unique identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Counterparty legal name\"\n        },\n        \"lei\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z0-9]{20}$\",\n          \"description\": \"Legal Entity\
  \ Identifier\"\n        }\n      }\n    },\n    \"RiskMeasures\": {\n      \"type\": \"object\",\n      \"description\": \"Position-level risk sensitivities and measures\",\n      \"properties\": {\n        \"delta\": {\n          \"type\": \"number\",\n          \"description\": \"First-order price sensitivity\"\n        },\n        \"gamma\": {\n          \"type\": \"number\",\n          \"description\": \"Second-order price sensitivity\"\n        },\n        \"vega\": {\n          \"type\": \"number\",\n          \"description\": \"Sensitivity to implied volatility\"\n        },\n        \"theta\": {\n          \"type\": \"number\",\n          \"description\": \"Time decay\"\n        },\n        \"rho\": {\n          \"type\": \"number\",\n          \"description\": \"Sensitivity to interest rate changes\"\n        },\n        \"pv01\": {\n          \"type\": \"number\",\n          \"description\": \"Price value of a basis point\"\n        },\n        \"cs01\": {\n          \"type\"\
  : \"number\",\n          \"description\": \"Credit spread sensitivity per basis point\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/murex/refs/heads/main/json-schema/murex-position-schema.json
tags:
- Capital Markets
- Enterprise Software
- Financial Services
- Fintech
- Risk Management
- Trading
title: Murex Position
---
