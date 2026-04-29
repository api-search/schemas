---
description: JSON Schema for a Broadridge Wealth Management securities position (holding) in a brokerage account.
layout: schema
name: Broadridge Position
properties_list:
- description: Unique position identifier
  name: positionId
  type: string
- description: Brokerage account number
  name: accountNumber
  type: string
- description: Committee on Uniform Securities Identification Procedures number
  name: cusip
  type: string
- description: Ticker symbol
  name: symbol
  type: string
- description: Full security name/description
  name: securityDescription
  type: string
- description: ''
  name: assetClass
  type: string
- description: Number of shares or units held
  name: quantity
  type: number
- description: Current price per share/unit
  name: price
  type: number
- description: Total market value (quantity * price)
  name: marketValue
  type: number
- description: Total cost basis for the position
  name: costBasis
  type: number
- description: Unrealized gain/loss (marketValue - costBasis)
  name: unrealizedGainLoss
  type: number
- description: Unrealized gain/loss as percentage of cost basis
  name: unrealizedGainLossPct
  type: number
- description: ''
  name: currency
  type: string
- description: Date the position data is as-of
  name: asOfDate
  type: string
provider_name: broadridge
provider_slug: broadridge
schema_file: json-schema/broadridge-position-schema.json
slug: broadridge-position
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/json-schema/broadridge-position-schema.json\",\n  \"title\": \"Broadridge Position\",\n  \"description\": \"JSON Schema for a Broadridge Wealth Management securities position (holding) in a brokerage account.\",\n  \"type\": \"object\",\n  \"required\": [\"positionId\", \"accountNumber\", \"symbol\", \"quantity\"],\n  \"properties\": {\n    \"positionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique position identifier\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Brokerage account number\"\n    },\n    \"cusip\": {\n      \"type\": \"string\",\n      \"description\": \"Committee on Uniform Securities Identification Procedures number\",\n      \"pattern\": \"^[A-Z0-9]{9}$\"\n    },\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Ticker symbol\"\n    },\n    \"securityDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Full security name/description\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"enum\": [\"Equity\", \"FixedIncome\", \"MutualFund\", \"ETF\", \"Options\", \"Cash\", \"Alternative\"]\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Number of shares or units held\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Current price per share/unit\",\n      \"minimum\": 0\n    },\n    \"marketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Total market value (quantity * price)\"\n    },\n    \"costBasis\": {\n      \"type\": \"number\",\n      \"description\": \"Total cost basis for the position\"\n    },\n    \"unrealizedGainLoss\": {\n      \"type\": \"number\",\n      \"description\": \"Unrealized gain/loss (marketValue - costBasis)\"\n    },\n    \"unrealizedGainLossPct\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"Unrealized gain/loss as percentage of cost basis\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"asOfDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the position data is as-of\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadridge/refs/heads/main/json-schema/broadridge-position-schema.json
tags: []
title: Broadridge Position
---
