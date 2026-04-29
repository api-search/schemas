---
description: List of Mileage Plan transactions
layout: schema
name: TransactionList
properties_list:
- description: Member number
  name: memberId
  type: string
- description: ''
  name: transactions
  type: array
- description: Total transaction count
  name: totalCount
  type: integer
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-mileage-plan-transaction-list-schema.json
slug: alaska-air-mileage-plan-transaction-list
source_filename: alaska-air-mileage-plan-transaction-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-transaction-list-schema.json\",\n  \"title\": \"TransactionList\",\n  \"description\": \"List of Mileage Plan transactions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memberId\": {\n      \"type\": \"string\",\n      \"description\": \"Member number\",\n      \"example\": \"12345678\"\n    },\n    \"transactions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Transaction\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total transaction count\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-transaction-list-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: TransactionList
---
