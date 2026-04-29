---
description: Response confirming partner miles credit
layout: schema
name: PartnerMilesResponse
properties_list:
- description: Unique transaction identifier
  name: transactionId
  type: string
- description: Member number
  name: memberId
  type: string
- description: Miles credited
  name: miles
  type: integer
- description: Updated mile balance
  name: newBalance
  type: integer
- description: Transaction status
  name: status
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-mileage-plan-partner-miles-response-schema.json
slug: alaska-air-mileage-plan-partner-miles-response
source_filename: alaska-air-mileage-plan-partner-miles-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-partner-miles-response-schema.json\",\n  \"title\": \"PartnerMilesResponse\",\n  \"description\": \"Response confirming partner miles credit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier\",\n      \"example\": \"TXN-111222\"\n    },\n    \"memberId\": {\n      \"type\": \"string\",\n      \"description\": \"Member number\",\n      \"example\": \"12345678\"\n    },\n    \"miles\": {\n      \"type\": \"integer\",\n      \"description\": \"Miles credited\",\n      \"example\": 500\n    },\n    \"newBalance\": {\n      \"type\": \"integer\",\n      \"description\": \"Updated mile balance\",\n      \"example\": 125500\n    },\n    \"status\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"Transaction status\",\n      \"enum\": [\n        \"credited\",\n        \"pending\",\n        \"rejected\"\n      ],\n      \"example\": \"credited\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-mileage-plan-partner-miles-response-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: PartnerMilesResponse
---
