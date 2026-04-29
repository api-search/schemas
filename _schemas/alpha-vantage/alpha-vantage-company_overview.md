---
description: Company fundamental data including financial ratios and business description
layout: schema
name: CompanyOverview
properties_list:
- description: Stock ticker symbol
  name: Symbol
  type: string
- description: Company name
  name: Name
  type: string
- description: Company business description
  name: Description
  type: string
- description: Stock exchange listing
  name: Exchange
  type: string
- description: Trading currency code
  name: Currency
  type: string
- description: Country of incorporation
  name: Country
  type: string
- description: Business sector
  name: Sector
  type: string
- description: Industry classification
  name: Industry
  type: string
- description: Total market capitalization in USD
  name: MarketCapitalization
  type: string
- description: Price-to-earnings ratio
  name: PERatio
  type: string
- description: Earnings per share (TTM)
  name: EPS
  type: string
- description: Annual dividend yield as decimal
  name: DividendYield
  type: string
- description: Beta coefficient relative to S&P 500
  name: Beta
  type: string
provider_name: Alpha Vantage
provider_slug: alpha-vantage
schema_file: json-schema/alpha-vantage-company_overview-schema.json
slug: alpha-vantage-company_overview
source_filename: alpha-vantage-company_overview-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.alphavantage.co/schemas/alpha-vantage-company_overview-schema.json\",\n  \"title\": \"CompanyOverview\",\n  \"type\": \"object\",\n  \"description\": \"Company fundamental data including financial ratios and business description\",\n  \"properties\": {\n    \"Symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Stock ticker symbol\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Company name\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Company business description\"\n    },\n    \"Exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Stock exchange listing\"\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"description\": \"Trading currency code\"\n    },\n    \"Country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of incorporation\"\n   \
  \ },\n    \"Sector\": {\n      \"type\": \"string\",\n      \"description\": \"Business sector\"\n    },\n    \"Industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry classification\"\n    },\n    \"MarketCapitalization\": {\n      \"type\": \"string\",\n      \"description\": \"Total market capitalization in USD\"\n    },\n    \"PERatio\": {\n      \"type\": \"string\",\n      \"description\": \"Price-to-earnings ratio\"\n    },\n    \"EPS\": {\n      \"type\": \"string\",\n      \"description\": \"Earnings per share (TTM)\"\n    },\n    \"DividendYield\": {\n      \"type\": \"string\",\n      \"description\": \"Annual dividend yield as decimal\"\n    },\n    \"Beta\": {\n      \"type\": \"string\",\n      \"description\": \"Beta coefficient relative to S&P 500\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alpha-vantage/refs/heads/main/json-schema/alpha-vantage-company_overview-schema.json
tags:
- Financial
- Market Data
- Stocks
- Technical Indicators
- Economic Data
- Sentiment Analysis
title: CompanyOverview
---
