---
description: A Speed Perks points transaction.
layout: schema
name: LoyaltyTransaction
properties_list:
- description: Transaction ID.
  name: id
  type: string
- description: Transaction type.
  name: type
  type: string
- description: Points earned or redeemed.
  name: points
  type: integer
- description: Transaction description.
  name: description
  type: string
- description: Transaction date.
  name: date
  type: string
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schema_file: json-schema/commerce-api-loyaltytransaction-schema.json
slug: commerce-api-loyaltytransaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoyaltyTransaction\",\n  \"description\": \"A Speed Perks points transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction ID.\",\n      \"example\": \"txn-001\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction type.\",\n      \"enum\": [\n        \"earn\",\n        \"redeem\",\n        \"expire\",\n        \"adjust\"\n      ]\n    },\n    \"points\": {\n      \"type\": \"integer\",\n      \"description\": \"Points earned or redeemed.\",\n      \"example\": 100\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction description.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Transaction date.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/json-schema/commerce-api-loyaltytransaction-schema.json
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
title: LoyaltyTransaction
---
