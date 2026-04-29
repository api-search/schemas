---
description: ''
layout: schema
name: Chase FDX Account
properties_list:
- description: ''
  name: accountId
  type: string
- description: ''
  name: accountType
  type: string
- description: ''
  name: accountCategory
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: currency
  type: string
- description: ''
  name: currentBalance
  type: number
- description: ''
  name: availableBalance
  type: number
- description: ''
  name: accountNumberDisplay
  type: string
- description: ''
  name: status
  type: string
provider_name: Chase
provider_slug: chase
schema_file: json-schema/chase-account-schema.json
slug: chase-account
source_filename: chase-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.chase.com/schemas/account.json\",\n  \"title\": \"Chase FDX Account\",\n  \"type\": \"object\",\n  \"required\": [\"accountId\", \"accountType\"],\n  \"properties\": {\n    \"accountId\": { \"type\": \"string\" },\n    \"accountType\": { \"type\": \"string\" },\n    \"accountCategory\": { \"type\": \"string\" },\n    \"displayName\": { \"type\": \"string\" },\n    \"currency\": { \"type\": \"string\" },\n    \"currentBalance\": { \"type\": \"number\" },\n    \"availableBalance\": { \"type\": \"number\" },\n    \"accountNumberDisplay\": { \"type\": \"string\" },\n    \"status\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/json-schema/chase-account-schema.json
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
title: Chase FDX Account
---
