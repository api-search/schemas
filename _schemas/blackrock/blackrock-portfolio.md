---
description: Schema for a portfolio record in the BlackRock Aladdin platform
layout: schema
name: BlackRock Aladdin Portfolio
properties_list:
- description: Unique portfolio identifier in Aladdin
  name: portfolioId
  type: string
- description: Display name of the portfolio
  name: portfolioName
  type: string
- description: Base currency (ISO 4217)
  name: currency
  type: string
- description: Total market value of the portfolio in base currency
  name: totalMarketValue
  type: number
- description: Valuation date
  name: asOfDate
  type: string
- description: Benchmark identifier for performance attribution
  name: benchmarkId
  type: string
- description: Portfolio manager identifier
  name: managerId
  type: string
- description: Investment strategy or mandate
  name: strategy
  type: string
- description: Holdings within the portfolio
  name: positions
  type: array
provider_name: BlackRock
provider_slug: blackrock
schema_file: json-schema/blackrock-portfolio-schema.json
slug: blackrock-portfolio
source_filename: blackrock-portfolio-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blackrock/main/json-schema/blackrock-portfolio-schema.json\",\n  \"title\": \"BlackRock Aladdin Portfolio\",\n  \"description\": \"Schema for a portfolio record in the BlackRock Aladdin platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique portfolio identifier in Aladdin\"\n    },\n    \"portfolioName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the portfolio\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Base currency (ISO 4217)\",\n      \"example\": \"USD\"\n    },\n    \"totalMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Total market value of the portfolio in base currency\"\n    },\n    \"asOfDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\
  ,\n      \"description\": \"Valuation date\"\n    },\n    \"benchmarkId\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark identifier for performance attribution\"\n    },\n    \"managerId\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio manager identifier\"\n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"description\": \"Investment strategy or mandate\"\n    },\n    \"positions\": {\n      \"type\": \"array\",\n      \"description\": \"Holdings within the portfolio\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Position\"\n      }\n    }\n  },\n  \"required\": [\"portfolioId\", \"portfolioName\", \"currency\", \"asOfDate\"],\n  \"$defs\": {\n    \"Position\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"securityId\": { \"type\": \"string\" },\n        \"identifier\": { \"type\": \"string\", \"description\": \"ISIN, CUSIP, or SEDOL\" },\n        \"quantity\": { \"type\": \"number\" },\n        \"marketValue\"\
  : { \"type\": \"number\" },\n        \"weight\": { \"type\": \"number\", \"description\": \"Weight as decimal (0-1)\" },\n        \"assetClass\": { \"type\": \"string\" },\n        \"currency\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/json-schema/blackrock-portfolio-schema.json
tags:
- Asset Management
- Finance
- FinTech
- Investment Management
- Portfolio Management
- Risk Analytics
title: BlackRock Aladdin Portfolio
---
