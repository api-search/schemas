---
description: Investment research data for a security
layout: schema
name: SecurityResearch
properties_list:
- description: Security identifier
  name: securityId
  type: string
- description: Ticker symbol
  name: ticker
  type: string
- description: Analyst consensus rating
  name: rating
  type: string
- description: Consensus price target
  name: priceTarget
  type: number
- description: Number of analysts covering the security
  name: analystCount
  type: integer
- description: Date of consensus calculation
  name: consensusDate
  type: string
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-investment-research-security-research-schema.json
slug: aladdin-studio-investment-research-security-research
source_filename: aladdin-studio-investment-research-security-research-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-investment-research-security-research-schema.json\",\n  \"title\": \"SecurityResearch\",\n  \"description\": \"Investment research data for a security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier\",\n      \"example\": \"US0378331005\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Ticker symbol\",\n      \"example\": \"AAPL\"\n    },\n    \"rating\": {\n      \"type\": \"string\",\n      \"description\": \"Analyst consensus rating\",\n      \"enum\": [\n        \"buy\",\n        \"hold\",\n        \"sell\"\n      ],\n      \"example\": \"buy\"\n    },\n    \"priceTarget\": {\n      \"type\": \"number\",\n      \"description\": \"Consensus price target\"\
  ,\n      \"example\": 225.0\n    },\n    \"analystCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of analysts covering the security\",\n      \"example\": 42\n    },\n    \"consensusDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of consensus calculation\",\n      \"example\": \"2026-04-19\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-investment-research-security-research-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: SecurityResearch
---
