---
description: Schema for a Blackstone alternative investment fund record
layout: schema
name: Blackstone Fund
properties_list:
- description: Unique fund identifier
  name: fundId
  type: string
- description: Full legal fund name
  name: fundName
  type: string
- description: Investment strategy
  name: strategy
  type: string
- description: Fund vintage year
  name: vintage
  type: integer
- description: Base currency (ISO 4217)
  name: currency
  type: string
- description: Total committed capital
  name: committedCapital
  type: number
- description: Capital called to date
  name: calledCapital
  type: number
- description: Net asset value
  name: nav
  type: number
- description: ''
  name: navDate
  type: string
- description: Internal rate of return
  name: irr
  type: number
- description: Multiple on invested capital
  name: moic
  type: number
- description: ''
  name: status
  type: string
provider_name: Blackstone
provider_slug: blackstone
schema_file: json-schema/blackstone-fund-schema.json
slug: blackstone-fund
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blackstone/main/json-schema/blackstone-fund-schema.json\",\n  \"title\": \"Blackstone Fund\",\n  \"description\": \"Schema for a Blackstone alternative investment fund record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fundId\": { \"type\": \"string\", \"description\": \"Unique fund identifier\" },\n    \"fundName\": { \"type\": \"string\", \"description\": \"Full legal fund name\" },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"enum\": [\"private_equity\", \"real_estate\", \"credit\", \"hedge_fund\", \"infrastructure\", \"life_sciences\"],\n      \"description\": \"Investment strategy\"\n    },\n    \"vintage\": { \"type\": \"integer\", \"description\": \"Fund vintage year\" },\n    \"currency\": { \"type\": \"string\", \"description\": \"Base currency (ISO 4217)\" },\n    \"committedCapital\": { \"type\": \"number\",\
  \ \"description\": \"Total committed capital\" },\n    \"calledCapital\": { \"type\": \"number\", \"description\": \"Capital called to date\" },\n    \"nav\": { \"type\": \"number\", \"description\": \"Net asset value\" },\n    \"navDate\": { \"type\": \"string\", \"format\": \"date\" },\n    \"irr\": { \"type\": \"number\", \"description\": \"Internal rate of return\" },\n    \"moic\": { \"type\": \"number\", \"description\": \"Multiple on invested capital\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"fundraising\", \"investing\", \"harvesting\", \"closed\"] }\n  },\n  \"required\": [\"fundId\", \"fundName\", \"strategy\", \"currency\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blackstone/refs/heads/main/json-schema/blackstone-fund-schema.json
tags:
- Alternative Assets
- Finance
- Investment Management
- Private Equity
- Real Estate
title: Blackstone Fund
---
