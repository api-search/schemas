---
description: ''
layout: schema
name: Schwab Account
properties_list:
- description: ''
  name: accountNumber
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: roundTrips
  type: integer
- description: ''
  name: isDayTrader
  type: boolean
- description: ''
  name: isClosingOnlyRestricted
  type: boolean
- description: ''
  name: positions
  type: array
- description: ''
  name: currentBalances
  type: object
provider_name: Charles Schwab
provider_slug: charles-schwab
schema_file: json-schema/charles-schwab-account-schema.json
slug: charles-schwab-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.schwab.com/schemas/account.json\",\n  \"title\": \"Schwab Account\",\n  \"type\": \"object\",\n  \"required\": [\"accountNumber\"],\n  \"properties\": {\n    \"accountNumber\": { \"type\": \"string\" },\n    \"type\": { \"type\": \"string\" },\n    \"roundTrips\": { \"type\": \"integer\" },\n    \"isDayTrader\": { \"type\": \"boolean\" },\n    \"isClosingOnlyRestricted\": { \"type\": \"boolean\" },\n    \"positions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"longQuantity\": { \"type\": \"number\" },\n          \"shortQuantity\": { \"type\": \"number\" },\n          \"marketValue\": { \"type\": \"number\" },\n          \"averagePrice\": { \"type\": \"number\" }\n        }\n      }\n    },\n    \"currentBalances\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cashBalance\": { \"\
  type\": \"number\" },\n        \"liquidationValue\": { \"type\": \"number\" },\n        \"availableFunds\": { \"type\": \"number\" },\n        \"buyingPower\": { \"type\": \"number\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/json-schema/charles-schwab-account-schema.json
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
title: Schwab Account
---
