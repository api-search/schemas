---
description: List of portfolio positions as of a date
layout: schema
name: PositionList
properties_list:
- description: Array of position objects
  name: positions
  type: array
- description: Portfolio identifier
  name: portfolioId
  type: string
- description: Position date
  name: asOfDate
  type: string
- description: Total portfolio market value
  name: totalMarketValue
  type: number
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-graph-position-list-schema.json
slug: aladdin-studio-graph-position-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-position-list-schema.json\",\n  \"title\": \"PositionList\",\n  \"description\": \"List of portfolio positions as of a date\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"positions\": {\n      \"type\": \"array\",\n      \"description\": \"Array of position objects\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Position\"\n      }\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio identifier\",\n      \"example\": \"PF-123456\"\n    },\n    \"asOfDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Position date\",\n      \"example\": \"2026-04-19\"\n    },\n    \"totalMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Total portfolio market value\"\
  ,\n      \"example\": 7800000.0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-position-list-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: PositionList
---
