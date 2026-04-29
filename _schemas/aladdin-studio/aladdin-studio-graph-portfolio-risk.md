---
description: Risk analytics for a portfolio computed by Aladdin's risk engine
layout: schema
name: PortfolioRisk
properties_list:
- description: Portfolio identifier
  name: portfolioId
  type: string
- description: Risk calculation date
  name: asOfDate
  type: string
- description: Annualized tracking error vs benchmark
  name: trackingError
  type: number
- description: 95% Value at Risk (1-day)
  name: var95
  type: number
- description: Portfolio beta vs benchmark
  name: beta
  type: number
- description: Annualized portfolio volatility
  name: volatility
  type: number
- description: Factor exposure breakdown
  name: factorExposures
  type: array
- description: Risk model used for calculation
  name: riskModel
  type: string
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-graph-portfolio-risk-schema.json
slug: aladdin-studio-graph-portfolio-risk
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-portfolio-risk-schema.json\",\n  \"title\": \"PortfolioRisk\",\n  \"description\": \"Risk analytics for a portfolio computed by Aladdin's risk engine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio identifier\",\n      \"example\": \"PF-123456\"\n    },\n    \"asOfDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Risk calculation date\",\n      \"example\": \"2026-04-19\"\n    },\n    \"trackingError\": {\n      \"type\": \"number\",\n      \"description\": \"Annualized tracking error vs benchmark\",\n      \"example\": 0.0342\n    },\n    \"var95\": {\n      \"type\": \"number\",\n      \"description\": \"95% Value at Risk (1-day)\",\n      \"example\"\
  : -0.0285\n    },\n    \"beta\": {\n      \"type\": \"number\",\n      \"description\": \"Portfolio beta vs benchmark\",\n      \"example\": 1.02\n    },\n    \"volatility\": {\n      \"type\": \"number\",\n      \"description\": \"Annualized portfolio volatility\",\n      \"example\": 0.152\n    },\n    \"factorExposures\": {\n      \"type\": \"array\",\n      \"description\": \"Factor exposure breakdown\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FactorExposure\"\n      }\n    },\n    \"riskModel\": {\n      \"type\": \"string\",\n      \"description\": \"Risk model used for calculation\",\n      \"example\": \"AXUS4\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-portfolio-risk-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: PortfolioRisk
---
