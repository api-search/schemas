---
description: Investment analytics and performance metrics for a portfolio
layout: schema
name: PortfolioAnalytics
properties_list:
- description: Portfolio identifier
  name: portfolioId
  type: string
- description: Analytics period start date
  name: fromDate
  type: string
- description: Analytics period end date
  name: toDate
  type: string
- description: Total portfolio return for the period
  name: totalReturn
  type: number
- description: Excess return vs benchmark
  name: excessReturn
  type: number
- description: Information ratio for the period
  name: informationRatio
  type: number
- description: Sharpe ratio for the period
  name: sharpeRatio
  type: number
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-investment-research-portfolio-analytics-schema.json
slug: aladdin-studio-investment-research-portfolio-analytics
source_filename: aladdin-studio-investment-research-portfolio-analytics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-investment-research-portfolio-analytics-schema.json\",\n  \"title\": \"PortfolioAnalytics\",\n  \"description\": \"Investment analytics and performance metrics for a portfolio\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio identifier\",\n      \"example\": \"PF-123456\"\n    },\n    \"fromDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Analytics period start date\",\n      \"example\": \"2026-01-01\"\n    },\n    \"toDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Analytics period end date\",\n      \"example\": \"2026-04-19\"\n    },\n    \"totalReturn\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Total portfolio return for the period\",\n      \"example\": 0.0485\n    },\n    \"excessReturn\": {\n      \"type\": \"number\",\n      \"description\": \"Excess return vs benchmark\",\n      \"example\": 0.0132\n    },\n    \"informationRatio\": {\n      \"type\": \"number\",\n      \"description\": \"Information ratio for the period\",\n      \"example\": 0.85\n    },\n    \"sharpeRatio\": {\n      \"type\": \"number\",\n      \"description\": \"Sharpe ratio for the period\",\n      \"example\": 1.24\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-investment-research-portfolio-analytics-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: PortfolioAnalytics
---
