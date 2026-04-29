---
description: A Speed Perks loyalty account.
layout: schema
name: LoyaltyAccount
properties_list:
- description: Loyalty account ID.
  name: accountId
  type: string
- description: Member ID number.
  name: memberId
  type: string
- description: Current points balance.
  name: pointsBalance
  type: integer
- description: Loyalty tier.
  name: tier
  type: string
- description: Dollar value of available rewards.
  name: rewardValue
  type: number
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-loyaltyaccount-schema.json
slug: commerce-api-loyaltyaccount
source_filename: commerce-api-loyaltyaccount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoyaltyAccount\",\n  \"description\": \"A Speed Perks loyalty account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Loyalty account ID.\",\n      \"example\": \"sp-001\"\n    },\n    \"memberId\": {\n      \"type\": \"string\",\n      \"description\": \"Member ID number.\",\n      \"example\": \"123456789\"\n    },\n    \"pointsBalance\": {\n      \"type\": \"integer\",\n      \"description\": \"Current points balance.\",\n      \"example\": 2500\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"description\": \"Loyalty tier.\",\n      \"enum\": [\n        \"Bronze\",\n        \"Silver\",\n        \"Gold\",\n        \"Platinum\"\n      ]\n    },\n    \"rewardValue\": {\n      \"type\": \"number\",\n      \"description\": \"Dollar value of available rewards.\",\n      \"example\": 5.0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-loyaltyaccount-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: LoyaltyAccount
---
