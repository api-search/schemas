---
description: Schema for a risk analytics report from BlackRock Aladdin
layout: schema
name: BlackRock Aladdin Risk Report
properties_list:
- description: ''
  name: reportId
  type: string
- description: ''
  name: portfolioId
  type: string
- description: ''
  name: asOfDate
  type: string
- description: ''
  name: currency
  type: string
- description: ''
  name: riskMetrics
  type: object
- description: ''
  name: factorExposures
  type: array
- description: ''
  name: stressTests
  type: array
provider_name: BlackRock
provider_slug: blackrock
schema_file: json-schema/blackrock-risk-report-schema.json
slug: blackrock-risk-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blackrock/main/json-schema/blackrock-risk-report-schema.json\",\n  \"title\": \"BlackRock Aladdin Risk Report\",\n  \"description\": \"Schema for a risk analytics report from BlackRock Aladdin\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": { \"type\": \"string\" },\n    \"portfolioId\": { \"type\": \"string\" },\n    \"asOfDate\": { \"type\": \"string\", \"format\": \"date\" },\n    \"currency\": { \"type\": \"string\" },\n    \"riskMetrics\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"var95\": { \"type\": \"number\", \"description\": \"95% Value at Risk\" },\n        \"var99\": { \"type\": \"number\", \"description\": \"99% Value at Risk\" },\n        \"expectedShortfall\": { \"type\": \"number\" },\n        \"annualizedVolatility\": { \"type\": \"number\" },\n        \"trackingError\": { \"type\": \"\
  number\" },\n        \"beta\": { \"type\": \"number\" },\n        \"durationYears\": { \"type\": \"number\" },\n        \"modifiedDuration\": { \"type\": \"number\" }\n      }\n    },\n    \"factorExposures\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"factorName\": { \"type\": \"string\" },\n          \"exposure\": { \"type\": \"number\" },\n          \"contribution\": { \"type\": \"number\" }\n        }\n      }\n    },\n    \"stressTests\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"scenarioName\": { \"type\": \"string\" },\n          \"pnlImpact\": { \"type\": \"number\" },\n          \"percentImpact\": { \"type\": \"number\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"reportId\", \"portfolioId\", \"asOfDate\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/json-schema/blackrock-risk-report-schema.json
tags:
- Asset Management
- Finance
- FinTech
- Investment Management
- Portfolio Management
- Risk Analytics
title: BlackRock Aladdin Risk Report
---
