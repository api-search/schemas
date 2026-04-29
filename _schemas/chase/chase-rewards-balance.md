---
description: ''
layout: schema
name: Chase Rewards Balance
properties_list:
- description: ''
  name: cardToken
  type: string
- description: ''
  name: pointsBalance
  type: integer
- description: ''
  name: cashValue
  type: number
- description: ''
  name: currency
  type: string
provider_name: Chase
provider_slug: chase
schema_file: json-schema/chase-rewards-balance-schema.json
slug: chase-rewards-balance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.chase.com/schemas/rewards-balance.json\",\n  \"title\": \"Chase Rewards Balance\",\n  \"type\": \"object\",\n  \"required\": [\"cardToken\", \"pointsBalance\"],\n  \"properties\": {\n    \"cardToken\": { \"type\": \"string\" },\n    \"pointsBalance\": { \"type\": \"integer\" },\n    \"cashValue\": { \"type\": \"number\" },\n    \"currency\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/json-schema/chase-rewards-balance-schema.json
tags:
- Account Aggregation
- Banking
- Consent
- Credit Cards
- FDX
- Financial Services
- Loyalty
- Open Banking
- Pay with Points
- Rewards
title: Chase Rewards Balance
---
