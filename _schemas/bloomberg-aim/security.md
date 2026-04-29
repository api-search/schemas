---
description: A financial security or instrument tracked within Bloomberg AIM, representing an equity, fixed income, derivative, or other tradeable asset.
layout: schema
name: Security
properties_list:
- description: Bloomberg ticker symbol (e.g., 'IBM US Equity')
  name: ticker
  type: string
- description: Full name of the security
  name: name
  type: string
- description: Financial Instrument Global Identifier (FIGI)
  name: figi
  type: string
- description: Composite FIGI for the security
  name: compositeFigi
  type: string
- description: International Securities Identification Number
  name: isin
  type: string
- description: Committee on Uniform Securities Identification Procedures number
  name: cusip
  type: string
- description: Stock Exchange Daily Official List number
  name: sedol
  type: string
- description: Bloomberg unique security identifier
  name: bloombergUniqueId
  type: string
- description: Asset class classification
  name: assetClass
  type: string
- description: Specific security type within the asset class
  name: securityType
  type: string
- description: Primary exchange where the security is listed
  name: exchange
  type: string
- description: Country of domicile (ISO 3166-1 alpha-2)
  name: country
  type: string
- description: Trading currency (ISO 4217)
  name: currency
  type: string
- description: Industry sector classification
  name: sector
  type: string
- description: Industry group within the sector
  name: industryGroup
  type: string
- description: Market capitalization in the trading currency
  name: marketCap
  type: number
- description: Last traded price
  name: lastPrice
  type: number
- description: Current bid price
  name: bidPrice
  type: number
- description: Current ask price
  name: askPrice
  type: number
- description: Trading volume for the current session
  name: volume
  type: integer
- description: Minimum trading lot size
  name: lotSize
  type: integer
- description: Coupon rate for fixed income securities (as a percentage)
  name: couponRate
  type: number
- description: Maturity date for fixed income and derivative securities
  name: maturityDate
  type: string
- description: Issue date of the security
  name: issueDate
  type: string
- description: Strike price for options
  name: strikePrice
  type: number
- description: Expiration date for options and futures
  name: expirationDate
  type: string
- description: Option type
  name: optionType
  type: string
- description: Ticker of the underlying security for derivatives
  name: underlyingTicker
  type: string
- description: Whether the security is actively trading
  name: active
  type: boolean
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/security.json
slug: security
source_filename: security.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://bloomberg.com/schemas/security.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Security\",\n  \"description\": \"A financial security or instrument tracked within Bloomberg AIM, representing an equity, fixed income, derivative, or other tradeable asset.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ticker\",\n    \"name\",\n    \"assetClass\"\n  ],\n  \"properties\": {\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg ticker symbol (e.g., 'IBM US Equity')\",\n      \"examples\": [\n        \"IBM US Equity\",\n        \"AAPL US Equity\",\n        \"T 3.5 02/15/2039 Corp\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the security\"\n    },\n    \"figi\": {\n      \"type\": \"string\",\n      \"description\": \"Financial Instrument Global Identifier (FIGI)\",\n      \"pattern\": \"^BBG[A-Z0-9]{9}$\"\n    },\n    \"\
  compositeFigi\": {\n      \"type\": \"string\",\n      \"description\": \"Composite FIGI for the security\",\n      \"pattern\": \"^BBG[A-Z0-9]{9}$\"\n    },\n    \"isin\": {\n      \"type\": \"string\",\n      \"description\": \"International Securities Identification Number\",\n      \"pattern\": \"^[A-Z]{2}[A-Z0-9]{9}[0-9]$\"\n    },\n    \"cusip\": {\n      \"type\": \"string\",\n      \"description\": \"Committee on Uniform Securities Identification Procedures number\",\n      \"pattern\": \"^[A-Z0-9]{9}$\"\n    },\n    \"sedol\": {\n      \"type\": \"string\",\n      \"description\": \"Stock Exchange Daily Official List number\",\n      \"pattern\": \"^[A-Z0-9]{7}$\"\n    },\n    \"bloombergUniqueId\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg unique security identifier\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class classification\",\n      \"enum\": [\n        \"Equity\",\n        \"Fixed Income\",\n \
  \       \"Commodity\",\n        \"Currency\",\n        \"Index\",\n        \"Mortgage\",\n        \"Municipal\",\n        \"Preferred\",\n        \"Money Market\",\n        \"Government\",\n        \"Corporate\",\n        \"Option\",\n        \"Future\",\n        \"Fund\",\n        \"ETF\"\n      ]\n    },\n    \"securityType\": {\n      \"type\": \"string\",\n      \"description\": \"Specific security type within the asset class\",\n      \"examples\": [\n        \"Common Stock\",\n        \"Corporate Bond\",\n        \"Call Option\",\n        \"Put Option\",\n        \"Future Contract\"\n      ]\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Primary exchange where the security is listed\",\n      \"examples\": [\n        \"NYSE\",\n        \"NASDAQ\",\n        \"LSE\",\n        \"TSE\"\n      ]\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of domicile (ISO 3166-1 alpha-2)\",\n      \"pattern\": \"^[A-Z]{2}$\"\
  \n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Trading currency (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"sector\": {\n      \"type\": \"string\",\n      \"description\": \"Industry sector classification\"\n    },\n    \"industryGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Industry group within the sector\"\n    },\n    \"marketCap\": {\n      \"type\": \"number\",\n      \"description\": \"Market capitalization in the trading currency\"\n    },\n    \"lastPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Last traded price\"\n    },\n    \"bidPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Current bid price\"\n    },\n    \"askPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Current ask price\"\n    },\n    \"volume\": {\n      \"type\": \"integer\",\n      \"description\": \"Trading volume for the current session\"\n    },\n    \"lotSize\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Minimum trading lot size\",\n      \"default\": 1\n    },\n    \"couponRate\": {\n      \"type\": \"number\",\n      \"description\": \"Coupon rate for fixed income securities (as a percentage)\"\n    },\n    \"maturityDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Maturity date for fixed income and derivative securities\"\n    },\n    \"issueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Issue date of the security\"\n    },\n    \"strikePrice\": {\n      \"type\": \"number\",\n      \"description\": \"Strike price for options\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Expiration date for options and futures\"\n    },\n    \"optionType\": {\n      \"type\": \"string\",\n      \"description\": \"Option type\",\n      \"enum\": [\n        \"Call\",\n        \"Put\"\n      ]\n  \
  \  },\n    \"underlyingTicker\": {\n      \"type\": \"string\",\n      \"description\": \"Ticker of the underlying security for derivatives\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the security is actively trading\",\n      \"default\": true\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/security.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Security
---
