---
description: An Aladdin portfolio with associated metadata
layout: schema
name: Portfolio
properties_list:
- description: Unique portfolio identifier
  name: portfolioId
  type: string
- description: Portfolio display name
  name: name
  type: string
- description: Base currency ISO code
  name: currency
  type: string
- description: Portfolio status
  name: status
  type: string
- description: Benchmark identifier
  name: benchmarkId
  type: string
- description: Portfolio inception date
  name: inceptionDate
  type: string
- description: Primary asset class
  name: assetClass
  type: string
- description: Investment strategy
  name: strategy
  type: string
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-graph-portfolio-schema.json
slug: aladdin-studio-graph-portfolio
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-portfolio-schema.json\",\n  \"title\": \"Portfolio\",\n  \"description\": \"An Aladdin portfolio with associated metadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique portfolio identifier\",\n      \"example\": \"PF-123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio display name\",\n      \"example\": \"Global Equity Fund\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Base currency ISO code\",\n      \"example\": \"USD\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio status\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"pending\"\n   \
  \   ],\n      \"example\": \"active\"\n    },\n    \"benchmarkId\": {\n      \"type\": \"string\",\n      \"description\": \"Benchmark identifier\",\n      \"example\": \"MSCI-WORLD\"\n    },\n    \"inceptionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Portfolio inception date\",\n      \"example\": \"2020-01-15\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Primary asset class\",\n      \"example\": \"Equity\"\n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"description\": \"Investment strategy\",\n      \"example\": \"Long Only\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-portfolio-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: Portfolio
---
