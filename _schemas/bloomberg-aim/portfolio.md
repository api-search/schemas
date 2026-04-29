---
description: An investment portfolio managed within Bloomberg AIM, containing positions across multiple securities with associated analytics and compliance attributes.
layout: schema
name: Portfolio
properties_list:
- description: Unique portfolio identifier within the AIM system
  name: portfolioId
  type: string
- description: Human-readable portfolio name
  name: name
  type: string
- description: Description of the portfolio strategy or purpose
  name: description
  type: string
- description: Classification of the portfolio
  name: portfolioType
  type: string
- description: Base reporting currency (ISO 4217)
  name: currency
  type: string
- description: Bloomberg ticker of the benchmark index
  name: benchmarkTicker
  type: string
- description: Portfolio manager responsible for investment decisions
  name: manager
  type: string
- description: Unique identifier for the portfolio manager
  name: managerId
  type: string
- description: Custodian institution for the portfolio's assets
  name: custodian
  type: string
- description: Account identifier at the custodian
  name: custodianAccountId
  type: string
- description: Date the portfolio was created
  name: inceptionDate
  type: string
- description: Current portfolio status
  name: status
  type: string
- description: Total market value of all positions in base currency
  name: totalMarketValue
  type: number
- description: Total cost basis of all positions in base currency
  name: totalCostBasis
  type: number
- description: Available cash balance in the portfolio
  name: cashBalance
  type: number
- description: Unrealized profit and loss across all open positions
  name: unrealizedPnL
  type: number
- description: Realized profit and loss from closed positions
  name: realizedPnL
  type: number
- description: Total return as a percentage since inception
  name: totalReturn
  type: number
- description: Year-to-date return as a percentage
  name: ytdReturn
  type: number
- description: Month-to-date return as a percentage
  name: mtdReturn
  type: number
- description: Current positions held in the portfolio
  name: positions
  type: array
- description: Asset allocation breakdown as percentage weights
  name: assetAllocation
  type: object
- description: Portfolio-level risk metrics
  name: riskMetrics
  type: object
- description: Portfolio compliance status
  name: complianceStatus
  type: string
- description: Custom tags for portfolio classification
  name: tags
  type: array
- description: Timestamp of the last portfolio update
  name: lastUpdated
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/portfolio.json
slug: portfolio
source_filename: portfolio.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://bloomberg.com/schemas/portfolio.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Portfolio\",\n  \"description\": \"An investment portfolio managed within Bloomberg AIM, containing positions across multiple securities with associated analytics and compliance attributes.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"portfolioId\",\n    \"name\"\n  ],\n  \"properties\": {\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique portfolio identifier within the AIM system\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable portfolio name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the portfolio strategy or purpose\"\n    },\n    \"portfolioType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the portfolio\",\n      \"enum\": [\n        \"Trading\"\
  ,\n        \"Model\",\n        \"Benchmark\",\n        \"Composite\",\n        \"Sleeve\",\n        \"Master\",\n        \"Sub-Account\"\n      ]\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Base reporting currency (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"benchmarkTicker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg ticker of the benchmark index\"\n    },\n    \"manager\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio manager responsible for investment decisions\"\n    },\n    \"managerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the portfolio manager\"\n    },\n    \"custodian\": {\n      \"type\": \"string\",\n      \"description\": \"Custodian institution for the portfolio's assets\"\n    },\n    \"custodianAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account identifier at the custodian\"\n    },\n    \"inceptionDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the portfolio was created\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current portfolio status\",\n      \"enum\": [\n        \"Active\",\n        \"Closed\",\n        \"Pending\",\n        \"Frozen\"\n      ],\n      \"default\": \"Active\"\n    },\n    \"totalMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Total market value of all positions in base currency\"\n    },\n    \"totalCostBasis\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost basis of all positions in base currency\"\n    },\n    \"cashBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Available cash balance in the portfolio\"\n    },\n    \"unrealizedPnL\": {\n      \"type\": \"number\",\n      \"description\": \"Unrealized profit and loss across all open positions\"\n    },\n    \"realizedPnL\": {\n      \"type\": \"number\",\n\
  \      \"description\": \"Realized profit and loss from closed positions\"\n    },\n    \"totalReturn\": {\n      \"type\": \"number\",\n      \"description\": \"Total return as a percentage since inception\"\n    },\n    \"ytdReturn\": {\n      \"type\": \"number\",\n      \"description\": \"Year-to-date return as a percentage\"\n    },\n    \"mtdReturn\": {\n      \"type\": \"number\",\n      \"description\": \"Month-to-date return as a percentage\"\n    },\n    \"positions\": {\n      \"type\": \"array\",\n      \"description\": \"Current positions held in the portfolio\",\n      \"items\": {\n        \"$ref\": \"https://bloomberg.com/schemas/position.json\"\n      }\n    },\n    \"assetAllocation\": {\n      \"type\": \"object\",\n      \"description\": \"Asset allocation breakdown as percentage weights\",\n      \"properties\": {\n        \"equity\": {\n          \"type\": \"number\",\n          \"description\": \"Percentage allocated to equities\"\n        },\n        \"fixedIncome\"\
  : {\n          \"type\": \"number\",\n          \"description\": \"Percentage allocated to fixed income\"\n        },\n        \"cash\": {\n          \"type\": \"number\",\n          \"description\": \"Percentage held in cash\"\n        },\n        \"alternatives\": {\n          \"type\": \"number\",\n          \"description\": \"Percentage allocated to alternative investments\"\n        },\n        \"commodities\": {\n          \"type\": \"number\",\n          \"description\": \"Percentage allocated to commodities\"\n        },\n        \"other\": {\n          \"type\": \"number\",\n          \"description\": \"Percentage in other asset classes\"\n        }\n      }\n    },\n    \"riskMetrics\": {\n      \"type\": \"object\",\n      \"description\": \"Portfolio-level risk metrics\",\n      \"properties\": {\n        \"beta\": {\n          \"type\": \"number\",\n          \"description\": \"Portfolio beta relative to benchmark\"\n        },\n        \"sharpeRatio\": {\n          \"type\"\
  : \"number\",\n          \"description\": \"Sharpe ratio measuring risk-adjusted return\"\n        },\n        \"volatility\": {\n          \"type\": \"number\",\n          \"description\": \"Annualized portfolio volatility (standard deviation)\"\n        },\n        \"trackingError\": {\n          \"type\": \"number\",\n          \"description\": \"Tracking error versus benchmark\"\n        },\n        \"valueAtRisk\": {\n          \"type\": \"number\",\n          \"description\": \"Value at Risk (95% confidence) in base currency\"\n        },\n        \"duration\": {\n          \"type\": \"number\",\n          \"description\": \"Modified duration for fixed income portfolios\"\n        },\n        \"convexity\": {\n          \"type\": \"number\",\n          \"description\": \"Convexity for fixed income portfolios\"\n        }\n      }\n    },\n    \"complianceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio compliance status\",\n      \"enum\": [\n        \"\
  Compliant\",\n        \"Warning\",\n        \"Violation\",\n        \"Pending Review\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Custom tags for portfolio classification\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last portfolio update\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/portfolio.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Portfolio
---
