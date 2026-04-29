---
description: ''
layout: schema
name: CommodityDetail
properties_list:
- description: Unique commodity identifier
  name: id
  type: string
- description: Commodity display name
  name: name
  type: string
- description: Commodity type
  name: type
  type: string
- description: Current market price
  name: currentPrice
  type: number
- description: Price currency
  name: currency
  type: string
- description: Price unit of measure
  name: unit
  type: string
- description: Date of price quote
  name: priceDate
  type: string
- description: 52-week high price
  name: weekHigh
  type: number
- description: 52-week low price
  name: weekLow
  type: number
- description: Daily trading volume in bushels
  name: volume
  type: integer
provider_name: Archer Daniels Midland
provider_slug: archer-daniels-midland
schema_file: json-schema/archer-daniels-midland-commodity-data-api-commodity-detail-schema.json
slug: archer-daniels-midland-commodity-data-api-commodity-detail
source_filename: archer-daniels-midland-commodity-data-api-commodity-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique commodity identifier\",\n      \"example\": \"CORN-US\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity display name\",\n      \"example\": \"Yellow Corn\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity type\",\n      \"enum\": [\n        \"corn\",\n        \"soybeans\",\n        \"wheat\",\n        \"canola\",\n        \"sorghum\",\n        \"barley\"\n      ],\n      \"example\": \"corn\"\n    },\n    \"currentPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Current market price\",\n      \"example\": 4.85\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Price currency\",\n      \"example\": \"USD\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Price unit of measure\",\n      \"example\"\
  : \"bushel\"\n    },\n    \"priceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of price quote\",\n      \"example\": \"2026-04-19\"\n    },\n    \"weekHigh\": {\n      \"type\": \"number\",\n      \"description\": \"52-week high price\",\n      \"example\": 5.1\n    },\n    \"weekLow\": {\n      \"type\": \"number\",\n      \"description\": \"52-week low price\",\n      \"example\": 4.72\n    },\n    \"volume\": {\n      \"type\": \"integer\",\n      \"description\": \"Daily trading volume in bushels\",\n      \"example\": 125000000\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-commodity-detail-schema.json\",\n  \"title\": \"CommodityDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archer-daniels-midland/refs/heads/main/json-schema/archer-daniels-midland-commodity-data-api-commodity-detail-schema.json
tags:
- Agriculture
- Food Processing
- Commodities
- Supply Chain
- Fortune 100
- Nutrition
title: CommodityDetail
---
