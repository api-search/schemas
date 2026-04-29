---
description: ''
layout: schema
name: Schwab Order
properties_list:
- description: ''
  name: orderId
  type: string
- description: ''
  name: session
  type: string
- description: ''
  name: duration
  type: string
- description: ''
  name: orderType
  type: string
- description: ''
  name: quantity
  type: number
- description: ''
  name: filledQuantity
  type: number
- description: ''
  name: remainingQuantity
  type: number
- description: ''
  name: orderStrategyType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: enteredTime
  type: string
- description: ''
  name: closeTime
  type: string
- description: ''
  name: orderLegCollection
  type: array
provider_name: Charles Schwab
provider_slug: charles-schwab
schema_file: json-schema/charles-schwab-order-schema.json
slug: charles-schwab-order
source_filename: charles-schwab-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.schwab.com/schemas/order.json\",\n  \"title\": \"Schwab Order\",\n  \"type\": \"object\",\n  \"required\": [\"orderType\", \"session\", \"duration\", \"orderStrategyType\"],\n  \"properties\": {\n    \"orderId\": { \"type\": \"string\" },\n    \"session\": {\n      \"type\": \"string\",\n      \"enum\": [\"NORMAL\", \"AM\", \"PM\", \"SEAMLESS\"]\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"enum\": [\"DAY\", \"GOOD_TILL_CANCEL\", \"FILL_OR_KILL\"]\n    },\n    \"orderType\": {\n      \"type\": \"string\",\n      \"enum\": [\"MARKET\", \"LIMIT\", \"STOP\", \"STOP_LIMIT\", \"TRAILING_STOP\"]\n    },\n    \"quantity\": { \"type\": \"number\" },\n    \"filledQuantity\": { \"type\": \"number\" },\n    \"remainingQuantity\": { \"type\": \"number\" },\n    \"orderStrategyType\": { \"type\": \"string\" },\n    \"status\": { \"type\": \"string\" },\n    \"enteredTime\"\
  : { \"type\": \"string\", \"format\": \"date-time\" },\n    \"closeTime\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"orderLegCollection\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"instruction\": {\n            \"type\": \"string\",\n            \"enum\": [\"BUY\", \"SELL\", \"BUY_TO_OPEN\", \"SELL_TO_CLOSE\", \"SELL_SHORT\", \"BUY_TO_COVER\"]\n          },\n          \"quantity\": { \"type\": \"number\" },\n          \"instrument\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"symbol\": { \"type\": \"string\" },\n              \"assetType\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/json-schema/charles-schwab-order-schema.json
tags:
- Accounts
- Banking
- Brokerage
- Financial Services
- Investing
- Market Data
- OAuth 2.0
- Orders
- Trading
title: Schwab Order
---
