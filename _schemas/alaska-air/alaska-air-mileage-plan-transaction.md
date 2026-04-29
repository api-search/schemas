---
description: A Mileage Plan mile earn or redeem transaction
layout: schema
name: Transaction
properties_list:
- description: Unique transaction identifier
  name: transactionId
  type: string
- description: Transaction type
  name: type
  type: string
- description: Miles earned or redeemed
  name: miles
  type: integer
- description: Transaction description
  name: description
  type: string
- description: Transaction date
  name: date
  type: string
- description: Partner name
  name: partner
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-mileage-plan-transaction-schema.json
slug: alaska-air-mileage-plan-transaction
source_filename: alaska-air-mileage-plan-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"A Mileage Plan mile earn or redeem transaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier\",\n      \"example\": \"TXN-987654\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction type\",\n      \"enum\": [\n        \"earn\",\n        \"redeem\"\n      ],\n      \"example\": \"earn\"\n    },\n    \"miles\": {\n      \"type\": \"integer\",\n      \"description\": \"Miles earned or redeemed\",\n      \"example\": 2500\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction description\",\n      \"example\": \"\
  Flight AS123 SEA-LAX\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Transaction date\",\n      \"example\": \"2026-04-19\"\n    },\n    \"partner\": {\n      \"type\": \"string\",\n      \"description\": \"Partner name\",\n      \"example\": \"Alaska Airlines\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-transaction-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: Transaction
---
