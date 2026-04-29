---
description: Schema for a limited partner investor account at Blackstone
layout: schema
name: Blackstone Investor Account
properties_list:
- description: ''
  name: accountId
  type: string
- description: ''
  name: investorName
  type: string
- description: ''
  name: investorType
  type: string
- description: ''
  name: currency
  type: string
- description: ''
  name: commitments
  type: array
- description: ''
  name: totalNav
  type: number
- description: ''
  name: totalDistributions
  type: number
- description: ''
  name: asOfDate
  type: string
provider_name: Blackstone
provider_slug: blackstone
schema_file: json-schema/blackstone-investor-account-schema.json
slug: blackstone-investor-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/blackstone/main/json-schema/blackstone-investor-account-schema.json\",\n  \"title\": \"Blackstone Investor Account\",\n  \"description\": \"Schema for a limited partner investor account at Blackstone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": { \"type\": \"string\" },\n    \"investorName\": { \"type\": \"string\" },\n    \"investorType\": {\n      \"type\": \"string\",\n      \"enum\": [\"pension_fund\", \"sovereign_wealth_fund\", \"endowment\", \"foundation\", \"insurance\", \"family_office\", \"hnwi\", \"other\"]\n    },\n    \"currency\": { \"type\": \"string\" },\n    \"commitments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fundId\": { \"type\": \"string\" },\n          \"committedAmount\": { \"type\": \"number\" },\n          \"calledAmount\"\
  : { \"type\": \"number\" },\n          \"distributedAmount\": { \"type\": \"number\" },\n          \"nav\": { \"type\": \"number\" }\n        }\n      }\n    },\n    \"totalNav\": { \"type\": \"number\" },\n    \"totalDistributions\": { \"type\": \"number\" },\n    \"asOfDate\": { \"type\": \"string\", \"format\": \"date\" }\n  },\n  \"required\": [\"accountId\", \"investorName\", \"currency\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/blackstone/refs/heads/main/json-schema/blackstone-investor-account-schema.json
tags:
- Alternative Assets
- Finance
- Investment Management
- Private Equity
- Real Estate
title: Blackstone Investor Account
---
